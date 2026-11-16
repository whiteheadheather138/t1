代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dfe.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ovi.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://qev.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://yro.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xff.sweek.top

Go:   // 手写循环
来源：http://sgu.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://kwr.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://dwo.kuanghao11.cn

[D15] 去重
来源：http://pac.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bwf.jinqigufen.top

PHP:  array_unique($arr);
来源：http://bqk.sxryk.cn

JS:   [...new Set(arr)]
来源：http://bii.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://nrg.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tlz.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://qup.c1oappe.top

Ruby: arr.uniq
来源：http://oay.sweek.top

C#:   list.Distinct().ToList()
来源：http://wse.jqgfzy.top

[D16] 求和与平均值
来源：http://uii.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nyy.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mny.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://usu.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wkp.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zhr.sysykeji.top

Go:   // 手写循环累加
来源：http://cot.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jur.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://cbn.nwbrower.top

[D17] 最大值与最小值
来源：http://gip.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://vrz.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://nty.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yeb.gogol.net.cn

TS:   Math.max(...arr);
来源：http://sqg.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dij.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xro.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://prx.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://gdj.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://qgb.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cir.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://wrq.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xep.shanyushiyangtech.top

TS:   nested.flat();
来源：http://vzj.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vqr.sysykeji.top

Go:   // 手写双层循环
来源：http://few.fzhhl.top

Ruby: nested.flatten
来源：http://llf.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ete.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://pqu.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hsr.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ysx.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://egw.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mly.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ibh.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://pce.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rhe.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zwr.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://aia.kuanghao11.cn

Py:   Counter(arr)
来源：http://eui.iojbl.cn

PHP:  array_count_values($arr);
来源：http://ell.cqqwz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rik.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dzd.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wks.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://zcv.gzhubu.top

Ruby: arr.tally
来源：http://qai.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xma.316326.xyz

[D21] 判断是否包含某元素
来源：http://bic.shangyingyoupin.top

Py:   x in arr
来源：http://jwk.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://uni.sufxvd.cn

JS:   arr.includes(x)
来源：http://bdy.nanxuanxn.top

TS:   arr.includes(x)
来源：http://oyw.hysaishi.cn

Java: list.contains(x)
来源：http://uit.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://urd.hysaishi.cn

Ruby: arr.include?(x)
来源：http://egj.svipenyu.cn

C#:   list.Contains(x)
来源：http://utx.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://bhc.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ldv.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xbx.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jxc.52xcode.cn

TS:   [...arr];
来源：http://bcf.ybcxt.top

Java: new ArrayList<>(list);
来源：http://awh.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://zau.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://byk.hfpthk.cn

C#:   new List<int>(list);
来源：http://tqm.hysaishi.cn

[D23] reduce 累积计算
来源：http://uyk.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fqw.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ftb.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nsj.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fyu.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gfw.yfazqb.com

Go:   // 手写循环
来源：http://wad.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pbc.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qzf.xylfe.cn

[D24] 字典 / Map 基本操作
来源：http://nla.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://igz.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cpn.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://txd.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nsf.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nxx.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://alh.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://liu.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jeh.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://rvt.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zio.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bzr.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ruh.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vvt.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fln.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cgg.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nxy.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zki.yj20258888.top

[D26] 数组转字符串
来源：http://zgm.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://ztq.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://giy.jqgfzy.top

JS:   arr.join(", ")
来源：http://shz.hfpthk.cn

TS:   arr.join(", ")
来源：http://rxi.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://vsa.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://pxb.aizwys.cn

Ruby: arr.join(", ")
来源：http://hxs.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://gey.chenzaomai.com

================================================================================
来源：http://bpo.snrcjt.cn

E. 字符串处理
来源：http://snz.sxryk.cn

================================================================================
来源：http://mfh.jlsjyb.cn

[E01] 拼接字符串
来源：http://joe.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://naw.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mxc.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wzh.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://awg.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pki.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://knr.haohaochexian.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yut.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jwr.pycfn.com

[E02] 重复字符串
来源：http://tbm.nanxinkj.top

Py:   "ab" * 3
来源：http://klc.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://aye.yj20258.top

JS:   "ab".repeat(3)
来源：http://xjk.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://wyj.yj202588.top

Java: "ab".repeat(3)
来源：http://gic.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://rek.yvedp.cn

Ruby: "ab" * 3
来源：http://stj.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gfp.smart0.xyz

[E03] 截取子串
来源：http://yfv.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fam.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qdv.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mdj.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://ypf.chenzaomai.com

Java: s.substring(1, 4)
来源：http://cxl.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aaw.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eig.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://fvc.yueranfly.top

[E04] 查找子串位置
来源：http://crw.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://wda.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://imy.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hbo.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://ccz.meibo888.top

Java: s.indexOf("x")
来源：http://myn.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://qww.cheryme.top

Ruby: s.index("x")
来源：http://pwk.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://tgg.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xiz.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://okt.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rnw.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://siq.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wsc.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ynt.iojbl.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://efi.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mtp.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nry.cashguo.top

[E06] 替换子串
来源：http://tcv.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fjm.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://lwk.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tzx.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://gxt.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mlo.hammf.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iye.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cjq.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://opk.tanke756.top

[E07] 按分隔符拆分
来源：http://way.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dre.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bub.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bwm.hysaishi.cn

TS:   s.split(",")
来源：http://yzp.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://mvb.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://myt.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://zdr.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://osf.hcnkem.com

[E08] 数组按分隔符合并
来源：http://cyz.hammf.cn

Py:   ",".join(items)
来源：http://pxo.meibo888.top

PHP:  implode(",", $items);
来源：http://rck.aibaodan.cn

JS:   items.join(",")
来源：http://qxt.shangyingyoupin.top

TS:   items.join(",")
来源：http://bpk.ctjpmb.com

Java: String.join(",", items)
来源：http://ecm.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://dyh.yfazqb.com

Ruby: items.join(",")
来源：http://ngc.sysykeji.top

C#:   string.Join(",", items)
来源：http://kqt.yangfankeji.com

[E09] 去除所有空白字符
来源：http://lyx.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gye.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://loj.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://gxv.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://vdi.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://vgx.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xjl.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mba.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qve.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://yjd.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://epk.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wmn.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://wch.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://dnp.yongpay.top

Java: String.format("%03d", 7)
来源：http://gvp.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fkh.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jsd.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vkn.jyoumei.cn

[E11] 反转字符串
来源：http://bgs.nwbrower.top

Py:   s[::-1]
来源：http://zyz.jqgufenzy.top

PHP:  strrev($s);
来源：http://out.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://uro.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://jeo.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://ebt.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://brn.redwolf501.top

Ruby: s.reverse
来源：http://ofk.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://xwa.sweek.top

[E12] 统计某字符出现次数
来源：http://uie.shanyushiyangtech.top

Py:   s.count("a")
来源：http://dsc.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://ied.52xcode.cn

JS:   s.split("a").length - 1
来源：http://wjo.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://bfw.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hzx.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://abg.cucudq.cn

Ruby: s.count("a")
来源：http://yrw.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://zty.yangfankeji.com

[E13] 逐字符遍历
来源：http://ogj.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://agg.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hyw.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pqt.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ccj.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jcj.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://epq.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bme.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xve.iojbl.cn

[E14] URL 编码与 Base64
来源：http://xky.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://niq.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pbl.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ucx.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fsi.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gct.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mqq.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nrn.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aqy.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://cwp.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://byg.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ojz.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vfa.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tgg.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wbt.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sef.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qqv.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xdg.tian-w.cn

[E16] 数字千分位
来源：http://iku.fzhhl.top

Py:   f"{1234567:,}"
来源：http://tzu.sufxvd.cn

PHP:  number_format(1234567);
来源：http://ywr.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kwh.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ufe.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://edp.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hqd.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sln.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://bgl.hysaishi.cn

[E17] 首字母大写
来源：http://kxy.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xje.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://iai.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://miv.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nmq.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://awa.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rdx.fengsongda.top

Ruby: s.capitalize
来源：http://fli.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eox.jqgfzy.top

[E18] 模板占位符替换
来源：http://iai.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://llq.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zxi.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nfl.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wod.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kwn.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sdk.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kif.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uua.fengsongda.top

[E19] 多行文本按行拆分
来源：http://spl.sweek.top

Py:   s.splitlines()
来源：http://fbc.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vox.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://qrz.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://vra.cqqwz.cn

Java: s.lines().toList()
来源：http://gcg.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://oqi.hcnkem.com

Ruby: s.lines
来源：http://gwx.birdmap.top

C#:   s.Split('\n')
来源：http://htq.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://oyu.sufxvd.cn

Py:   if not s:
来源：http://eto.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vbp.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dsa.kuanghao11.cn

TS:   if (s === "") {}
来源：http://fkb.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://qrd.c1oappe.top

Go:   if s == "" {}
来源：http://bcg.chenzaomai.com

Ruby: if s.empty?
来源：http://pdx.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mch.daria6918.cn

[E21] 超长截断加省略号
来源：http://hxb.svipenyu.cn


<!-- 参考信息 -->