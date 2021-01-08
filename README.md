# Master-PiB-Thyme

## S0_filtering_data file:
df_snp_filtered.t.vulgaris.5
df_snp_filtered.t.embergeri.5
df_genotype_filtered.t.vulgaris.5
df_genotype_filtered.t.embergeri.5   
these files were created after filtration by using 0.5 cutoff.

## S1_finding_polymorphism file:
df_only_poly_t.vulgaris.5: contains snps that found only in t.vulgaris with ancestral/derived information
df_only_poly_t.embergeri.5: contains snps that found only in t.embergeri
df_merged_polymorphisms.5: merged file of df_only_poly_t.vulgaris.5 and df_only_poly_t.embergeri.5 with anc/der info and only snp info
df_shared_poly.5: shared polymorphism data

only_2s.5: contigs that have 2s for all samples of t.embergeri
only_0s.5: contigs that have 0s for all samples of t.embergeri

## S3_Plots_(DAF_MAF_Prob_of_shared_allele) File:
-Derived allele freq distribution by using df_only_poly_t.vulgaris.5 data
-Minor allele freq dist of df_shared_polymorphisms data
-high frequency distribution only for vulgaris polymorphisms
n_high_freq_poly: number of high freq snps (>0.5) per contig

## S5_contigs_of_interest
contig_of_interest file contains contigs that have association with chemotypes and environment and their lengths

## S6_tajimaD_Htest
calculation of the tajimaD (for both df_only_poly.t.vulgaris and df_merged_poly) and H statistics (for df_only_poly.t.vulgaris)
contigs of interest were indicated on the plot

## S6b_site-specificTajimaD
Tajima test per site

## S7_Fst 
calculation Fst values per contig by using shared polymorphisms data
then it compared with percentage of shared poly per contig

## syn_nonsyn files
syn_nonsyn file is about finding nonsynoymous snps positions of contig of interest, whereas syn_nonsyn_allcontigs file is for all contigs. These were implementated by python. 

## S10_all_contigs_syn_nonsyn
Adding information about synonymous and nonsynoymous to the SNP data based on the table created In python.

## S11_MK_Test_all_contigs
Applying MK test all contigs by using syn-nonsyn info. Plot for distribution of NI and DoS.
Contig_of_interest_results rds file contains information about theta values, H.test, TajimaD, Fst, neutrality index and Its p value, and direction of selection 

