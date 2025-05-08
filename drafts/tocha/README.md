# Dataset 'Corpus of Tocharian (A) texts'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/toch/tocha/tocha.htm).

* URL: https://github.com/TITUS-2-0/tocharian/tree/main/drafts/tocha/
* version: unreleased
* date: 2025-04-22

## Citation
```text
Digital version of Corpus of Tocharian (A) texts (draft version). By: Jost Gippert, Katharina Kupfer, Florian Matter, P. Olivier, Tatsushi Tamai. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/tocharian/tree/main/drafts/tocha/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Manuscript | `div@manuscript` | Automatically translated into named div |
| Part | `div@part` | Automatically translated into named div |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=xto-Latn)
  body
    div (@data-level=1, @n, @type=manuscript, @xml:id) (multiple)
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        ab (@type=line-wrapper, @xml:id) (multiple)
          choice (multiple)
            orig (multiple)
              [foreign (@xml:lang=deu-Latn | san-Latn-x-buddhist-syllabic | san-Latn-x-buddhist-tld | xto-Latn-x-syllabic) (multiple)]
            reg (multiple)
              [foreign (@xml:lang=deu-Latn | san-Latn-x-buddhist-syllabic | san-Latn-x-buddhist-tld | xto-Latn-x-syllabic) (multiple)]
          [lb (@n) (multiple)]
        ab (@type=line-wrapper, @xml:id) (multiple)
          [lb (@n) (multiple)]
          [foreign (@xml:lang=deu-Latn | san-Latn-x-buddhist-syllabic | san-Latn-x-buddhist-tld | xto-Latn-x-syllabic) (multiple)]
        [milestone (@facs=#facs-1 | #facs-10 | #facs-100 | #facs-101 | #facs-102 | #facs-103 | #facs-104 | #facs-106 | #facs-107 | #facs-108 | #facs-109 | #facs-11 | #facs-110 | #facs-112 | #facs-113 | #facs-114 | #facs-115 | #facs-116 | #facs-117 | #facs-118 | #facs-119 | #facs-12 | #facs-120 | #facs-121 | #facs-122 | #facs-123 | #facs-124 | #facs-125 | #facs-126 | #facs-127 | #facs-128 | #facs-129 | #facs-13 | #facs-130 | #facs-131 | #facs-132 | #facs-133 | #facs-134 | #facs-136 | #facs-137 | #facs-138 | #facs-139 | #facs-14 | #facs-140 | #facs-141 | #facs-143 | #facs-144 | #facs-145 | #facs-146 | #facs-147 | #facs-148 | #facs-149 | #facs-15 | #facs-150 | #facs-151 | #facs-152 | #facs-153 | #facs-154 | #facs-155 | #facs-156 | #facs-157 | #facs-158 | #facs-159 | #facs-16 | #facs-161 | #facs-162 | #facs-163 | #facs-164 | #facs-165 | #facs-166 | #facs-167 | #facs-168 | #facs-169 | #facs-17 | #facs-170 | #facs-173 | #facs-174 | #facs-175 | #facs-176 | #facs-179 | #facs-18 | #facs-180 | #facs-181 | #facs-182 | #facs-186 | #facs-187 | #facs-188 | #facs-189 | #facs-19 | #facs-191 | #facs-192 | #facs-193 | #facs-194 | #facs-195 | #facs-196 | #facs-2 | #facs-20 | #facs-204 | #facs-205 | #facs-206 | #facs-207 | #facs-208 | #facs-209 | #facs-21 | #facs-210 | #facs-211 | #facs-212 | #facs-213 | #facs-214 | #facs-215 | #facs-216 | #facs-218 | #facs-219 | #facs-22 | #facs-220 | #facs-221 | #facs-222 | #facs-223 | #facs-224 | #facs-225 | #facs-226 | #facs-227 | #facs-228 | #facs-229 | #facs-23 | #facs-230 | #facs-231 | #facs-232 | #facs-233 | #facs-234 | #facs-235 | #facs-236 | #facs-237 | #facs-238 | #facs-239 | #facs-24 | #facs-240 | #facs-241 | #facs-242 | #facs-243 | #facs-244 | #facs-245 | #facs-246 | #facs-247 | #facs-248 | #facs-249 | #facs-25 | #facs-250 | #facs-251 | #facs-252 | #facs-253 | #facs-254 | #facs-255 | #facs-256 | #facs-257 | #facs-258 | #facs-259 | #facs-26 | #facs-260 | #facs-261 | #facs-262 | #facs-263 | #facs-265 | #facs-266 | #facs-267 | #facs-269 | #facs-27 | #facs-270 | #facs-271 | #facs-272 | #facs-273 | #facs-274 | #facs-275 | #facs-276 | #facs-277 | #facs-278 | #facs-279 | #facs-28 | #facs-281 | #facs-282 | #facs-283 | #facs-284 | #facs-285 | #facs-286 | #facs-287 | #facs-288 | #facs-289 | #facs-29 | #facs-290 | #facs-291 | #facs-292 | #facs-293 | #facs-294 | #facs-295 | #facs-296 | #facs-297 | #facs-298 | #facs-299 | #facs-3 | #facs-30 | #facs-300 | #facs-301 | #facs-302 | #facs-303 | #facs-304 | #facs-305 | #facs-306 | #facs-307 | #facs-309 | #facs-31 | #facs-310 | #facs-311 | #facs-312 | #facs-313 | #facs-314 | #facs-315 | #facs-316 | #facs-317 | #facs-318 | #facs-319 | #facs-32 | #facs-320 | #facs-321 | #facs-322 | #facs-323 | #facs-324 | #facs-325 | #facs-326 | #facs-327 | #facs-328 | #facs-329 | #facs-33 | #facs-330 | #facs-331 | #facs-332 | #facs-333 | #facs-334 | #facs-335 | #facs-336 | #facs-337 | #facs-338 | #facs-339 | #facs-34 | #facs-340 | #facs-341 | #facs-342 | #facs-343 | #facs-344 | #facs-346 | #facs-347 | #facs-348 | #facs-349 | #facs-35 | #facs-350 | #facs-351 | #facs-352 | #facs-353 | #facs-354 | #facs-355 | #facs-356 | #facs-357 | #facs-358 | #facs-359 | #facs-36 | #facs-360 | #facs-361 | #facs-362 | #facs-363 | #facs-364 | #facs-365 | #facs-366 | #facs-367 | #facs-368 | #facs-369 | #facs-37 | #facs-370 | #facs-371 | #facs-372 | #facs-373 | #facs-374 | #facs-375 | #facs-376 | #facs-377 | #facs-378 | #facs-379 | #facs-38 | #facs-380 | #facs-381 | #facs-382 | #facs-383 | #facs-384 | #facs-385 | #facs-386 | #facs-387 | #facs-388 | #facs-389 | #facs-39 | #facs-390 | #facs-391 | #facs-392 | #facs-393 | #facs-394 | #facs-395 | #facs-396 | #facs-397 | #facs-398 | #facs-399 | #facs-4 | #facs-40 | #facs-400 | #facs-401 | #facs-402 | #facs-403 | #facs-404 | #facs-405 | #facs-406 | #facs-407 | #facs-408 | #facs-41 | #facs-410 | #facs-411 | #facs-412 | #facs-413 | #facs-414 | #facs-415 | #facs-416 | #facs-417 | #facs-418 | #facs-419 | #facs-42 | #facs-420 | #facs-421 | #facs-422 | #facs-423 | #facs-424 | #facs-425 | #facs-426 | #facs-427 | #facs-428 | #facs-429 | #facs-43 | #facs-430 | #facs-431 | #facs-432 | #facs-433 | #facs-434 | #facs-435 | #facs-436 | #facs-439 | #facs-44 | #facs-440 | #facs-444 | #facs-445 | #facs-446 | #facs-447 | #facs-448 | #facs-449 | #facs-45 | #facs-450 | #facs-451 | #facs-452 | #facs-453 | #facs-454 | #facs-455 | #facs-456 | #facs-457 | #facs-458 | #facs-459 | #facs-46 | #facs-460 | #facs-462 | #facs-464 | #facs-465 | #facs-466 | #facs-467 | #facs-468 | #facs-469 | #facs-47 | #facs-470 | #facs-471 | #facs-472 | #facs-473 | #facs-474 | #facs-475 | #facs-476 | #facs-477 | #facs-478 | #facs-479 | #facs-48 | #facs-480 | #facs-481 | #facs-482 | #facs-483 | #facs-484 | #facs-485 | #facs-486 | #facs-487 | #facs-488 | #facs-489 | #facs-49 | #facs-490 | #facs-491 | #facs-492 | #facs-493 | #facs-494 | #facs-495 | #facs-496 | #facs-497 | #facs-498 | #facs-499 | #facs-5 | #facs-50 | #facs-500 | #facs-501 | #facs-502 | #facs-503 | #facs-504 | #facs-505 | #facs-506 | #facs-507 | #facs-508 | #facs-509 | #facs-51 | #facs-510 | #facs-511 | #facs-512 | #facs-513 | #facs-514 | #facs-515 | #facs-516 | #facs-517 | #facs-518 | #facs-519 | #facs-52 | #facs-520 | #facs-521 | #facs-522 | #facs-523 | #facs-524 | #facs-525 | #facs-526 | #facs-527 | #facs-528 | #facs-529 | #facs-53 | #facs-530 | #facs-531 | #facs-532 | #facs-533 | #facs-534 | #facs-535 | #facs-536 | #facs-537 | #facs-538 | #facs-539 | #facs-54 | #facs-540 | #facs-541 | #facs-542 | #facs-543 | #facs-544 | #facs-545 | #facs-546 | #facs-547 | #facs-548 | #facs-549 | #facs-55 | #facs-550 | #facs-551 | #facs-552 | #facs-553 | #facs-554 | #facs-555 | #facs-556 | #facs-557 | #facs-558 | #facs-559 | #facs-56 | #facs-560 | #facs-561 | #facs-562 | #facs-563 | #facs-564 | #facs-565 | #facs-566 | #facs-567 | #facs-568 | #facs-569 | #facs-57 | #facs-570 | #facs-571 | #facs-572 | #facs-573 | #facs-574 | #facs-575 | #facs-576 | #facs-577 | #facs-578 | #facs-579 | #facs-58 | #facs-580 | #facs-581 | #facs-582 | #facs-583 | #facs-584 | #facs-585 | #facs-586 | #facs-587 | #facs-588 | #facs-589 | #facs-59 | #facs-591 | #facs-592 | #facs-593 | #facs-594 | #facs-595 | #facs-596 | #facs-597 | #facs-598 | #facs-599 | #facs-6 | #facs-60 | #facs-601 | #facs-602 | #facs-603 | #facs-604 | #facs-605 | #facs-606 | #facs-607 | #facs-608 | #facs-609 | #facs-61 | #facs-610 | #facs-611 | #facs-612 | #facs-613 | #facs-614 | #facs-615 | #facs-616 | #facs-617 | #facs-618 | #facs-619 | #facs-62 | #facs-620 | #facs-621 | #facs-622 | #facs-623 | #facs-624 | #facs-625 | #facs-626 | #facs-627 | #facs-628 | #facs-629 | #facs-63 | #facs-630 | #facs-631 | #facs-632 | #facs-633 | #facs-634 | #facs-635 | #facs-636 | #facs-637 | #facs-638 | #facs-639 | #facs-64 | #facs-640 | #facs-641 | #facs-642 | #facs-643 | #facs-644 | #facs-645 | #facs-646 | #facs-647 | #facs-648 | #facs-649 | #facs-65 | #facs-651 | #facs-652 | #facs-653 | #facs-654 | #facs-655 | #facs-656 | #facs-657 | #facs-658 | #facs-659 | #facs-66 | #facs-660 | #facs-661 | #facs-662 | #facs-663 | #facs-664 | #facs-665 | #facs-666 | #facs-667 | #facs-668 | #facs-669 | #facs-67 | #facs-670 | #facs-671 | #facs-672 | #facs-673 | #facs-674 | #facs-675 | #facs-676 | #facs-677 | #facs-678 | #facs-679 | #facs-68 | #facs-680 | #facs-681 | #facs-682 | #facs-683 | #facs-684 | #facs-685 | #facs-686 | #facs-687 | #facs-688 | #facs-689 | #facs-69 | #facs-690 | #facs-691 | #facs-692 | #facs-693 | #facs-694 | #facs-695 | #facs-696 | #facs-697 | #facs-698 | #facs-699 | #facs-7 | #facs-70 | #facs-700 | #facs-701 | #facs-702 | #facs-703 | #facs-704 | #facs-705 | #facs-706 | #facs-707 | #facs-708 | #facs-709 | #facs-71 | #facs-710 | #facs-711 | #facs-712 | #facs-713 | #facs-714 | #facs-715 | #facs-716 | #facs-717 | #facs-718 | #facs-719 | #facs-72 | #facs-720 | #facs-721 | #facs-722 | #facs-723 | #facs-724 | #facs-725 | #facs-726 | #facs-727 | #facs-728 | #facs-729 | #facs-73 | #facs-730 | #facs-731 | #facs-732 | #facs-733 | #facs-734 | #facs-735 | #facs-736 | #facs-737 | #facs-738 | #facs-739 | #facs-74 | #facs-740 | #facs-741 | #facs-742 | #facs-743 | #facs-744 | #facs-745 | #facs-746 | #facs-747 | #facs-748 | #facs-749 | #facs-75 | #facs-750 | #facs-751 | #facs-752 | #facs-753 | #facs-754 | #facs-755 | #facs-756 | #facs-757 | #facs-758 | #facs-759 | #facs-76 | #facs-760 | #facs-761 | #facs-762 | #facs-763 | #facs-764 | #facs-765 | #facs-766 | #facs-767 | #facs-768 | #facs-769 | #facs-77 | #facs-770 | #facs-771 | #facs-772 | #facs-773 | #facs-774 | #facs-775 | #facs-776 | #facs-777 | #facs-778 | #facs-779 | #facs-78 | #facs-780 | #facs-781 | #facs-782 | #facs-783 | #facs-784 | #facs-785 | #facs-786 | #facs-787 | #facs-788 | #facs-789 | #facs-79 | #facs-790 | #facs-791 | #facs-792 | #facs-793 | #facs-794 | #facs-795 | #facs-796 | #facs-797 | #facs-798 | #facs-799 | #facs-8 | #facs-80 | #facs-800 | #facs-801 | #facs-802 | #facs-803 | #facs-804 | #facs-805 | #facs-806 | #facs-807 | #facs-808 | #facs-809 | #facs-81 | #facs-810 | #facs-811 | #facs-812 | #facs-813 | #facs-814 | #facs-815 | #facs-816 | #facs-817 | #facs-818 | #facs-819 | #facs-82 | #facs-820 | #facs-821 | #facs-822 | #facs-823 | #facs-824 | #facs-825 | #facs-826 | #facs-827 | #facs-828 | #facs-829 | #facs-83 | #facs-830 | #facs-831 | #facs-832 | #facs-833 | #facs-834 | #facs-835 | #facs-836 | #facs-837 | #facs-838 | #facs-839 | #facs-84 | #facs-840 | #facs-841 | #facs-842 | #facs-843 | #facs-844 | #facs-845 | #facs-846 | #facs-847 | #facs-848 | #facs-849 | #facs-85 | #facs-850 | #facs-851 | #facs-852 | #facs-853 | #facs-854 | #facs-855 | #facs-856 | #facs-857 | #facs-858 | #facs-859 | #facs-86 | #facs-860 | #facs-861 | #facs-862 | #facs-863 | #facs-864 | #facs-865 | #facs-866 | #facs-867 | #facs-868 | #facs-869 | #facs-87 | #facs-870 | #facs-871 | #facs-872 | #facs-873 | #facs-874 | #facs-875 | #facs-876 | #facs-877 | #facs-878 | #facs-879 | #facs-88 | #facs-880 | #facs-881 | #facs-882 | #facs-883 | #facs-884 | #facs-885 | #facs-886 | #facs-887 | #facs-888 | #facs-889 | #facs-89 | #facs-890 | #facs-891 | #facs-892 | #facs-893 | #facs-894 | #facs-895 | #facs-896 | #facs-897 | #facs-898 | #facs-899 | #facs-9 | #facs-90 | #facs-900 | #facs-901 | #facs-902 | #facs-903 | #facs-904 | #facs-905 | #facs-906 | #facs-907 | #facs-908 | #facs-909 | #facs-91 | #facs-910 | #facs-911 | #facs-912 | #facs-913 | #facs-92 | #facs-93 | #facs-94 | #facs-95 | #facs-96 | #facs-97 | #facs-98 | #facs-99, @n, @unit=ref, @xml:id) (multiple)]
        [note (@xml:id, @xml:lang=deu-Latn) (multiple)]
        [milestone (@facs=#facs-105 | #facs-111 | #facs-135 | #facs-142 | #facs-171 | #facs-172 | #facs-177 | #facs-178 | #facs-183 | #facs-184 | #facs-185 | #facs-190 | #facs-197 | #facs-198 | #facs-199 | #facs-200 | #facs-201 | #facs-202 | #facs-203 | #facs-217 | #facs-264 | #facs-268 | #facs-280 | #facs-308 | #facs-345 | #facs-409 | #facs-437 | #facs-438 | #facs-441 | #facs-442 | #facs-443 | #facs-461 | #facs-463 | #facs-590 | #facs-600 | #facs-650, @unit=ref, @xml:id) (multiple)]
        [note (@xml:id)]
      [note (@xml:id, @xml:lang=deu-Latn | xto-Latn-x-syllabic) (multiple)]
        [note (@xml:id, @xml:lang=deu-Latn)]
      [milestone (@facs=#facs-160, @unit=ref, @xml:id)]
    div (@data-level=1, @n, @type=manuscript, @xml:id)
      [note (@xml:id, @xml:lang=deu-Latn) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="634" xml:id="manuscript-1" type="manuscript" data-level="1">
				<note xml:id="manuscript-1-note-1" xml:lang="deu-Latn">No._1 = T_III_Š_72.1</note>
				<note xml:id="manuscript-1-note-2" xml:lang="deu-Latn">THT 0634</note>
				<note xml:id="manuscript-1-note-3" xml:lang="deu-Latn">Trägt auf der Rückseite die Blattzahl 65.</note>
				<div n="1a" xml:id="manuscript-1-part-1" type="part" data-level="2">
					<milestone facs="#facs-913" unit="ref" n="r" xml:id="manuscript-1-part-1-milestone-1"/>
					<ab type="line-wrapper" xml:id="manuscript-1-part-1-ab-1">
						<lb n="1"/>
						<choice>
							<orig>(kā)su1 ñoM\ klyu tsraṣiśśi śäK\ KAlymentwaṃ SAtkaTAR\ : yärK\ ynāñmune nam poto tsraṣṣuneyā PùKAṢ KAl(pnā)-</orig>
							<reg>
								<foreign xml:lang="xto-Latn-x-syllabic">su ño-M\ klyu tsra-ṣi-śśi śä-K\ KA-lyme-ntwaṃ [SA]-tka-TA-R\ : yä-rK\ ynā-ñmu-ne na-m^po-to tsra-ṣṣu-ne-yā PùKA-Ṣ^KA-l+</foreign>
  ...
```
