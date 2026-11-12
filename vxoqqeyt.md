代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qdj.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wuz.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://zrg.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://jod.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ngk.kuanghao11.cn

Go:   // 手写循环
来源：http://vtk.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mlv.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://woq.aibaodan.cn

[D15] 去重
来源：http://dhe.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://geb.aibaodan.cn

PHP:  array_unique($arr);
来源：http://ofo.birdmap.top

JS:   [...new Set(arr)]
来源：http://itg.daria6918.cn

TS:   [...new Set(arr)]
来源：http://alw.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kfx.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://ybb.smart0.xyz

Ruby: arr.uniq
来源：http://yhx.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://pcs.quarkkingdee.top

[D16] 求和与平均值
来源：http://xmr.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jmn.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ckz.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nrc.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rgk.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zyk.ehwqpu.com

Go:   // 手写循环累加
来源：http://ttv.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nqi.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://een.gotoacloud.top

[D17] 最大值与最小值
来源：http://vuv.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://ojm.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://tzk.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tmq.zhengqikj.top

TS:   Math.max(...arr);
来源：http://vyo.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kuy.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qws.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://cpf.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://fqs.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://jqu.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rar.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://xom.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://giy.yj202588.top

TS:   nested.flat();
来源：http://sss.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jux.vehdjk.com

Go:   // 手写双层循环
来源：http://icf.yj20258888.top

Ruby: nested.flatten
来源：http://yam.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vls.yj20258888.top

[D19] 按字段分组
来源：http://fok.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fcp.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://brc.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mnz.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://hfb.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://avl.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://gfu.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ymf.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uqa.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://pwy.sweek.top

Py:   Counter(arr)
来源：http://qmb.yongpay.top

PHP:  array_count_values($arr);
来源：http://ply.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oiv.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yls.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nmj.yonumen.top

Go:   // 手写 map[T]int
来源：http://off.zhixingplan.top

Ruby: arr.tally
来源：http://tor.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gdp.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://wwg.havefunace.top

Py:   x in arr
来源：http://ksm.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://gzk.cashguo.top

JS:   arr.includes(x)
来源：http://tae.fengsongda.top

TS:   arr.includes(x)
来源：http://kxw.zdqjudy.top

Java: list.contains(x)
来源：http://mds.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://jku.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://jzx.guowangkeji.top

C#:   list.Contains(x)
来源：http://sxr.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://lbs.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vnn.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jdr.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fud.epnwcf.com

TS:   [...arr];
来源：http://ijd.ydzc1.top

Java: new ArrayList<>(list);
来源：http://jsj.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://qfa.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://amf.quarkkingdee.top

C#:   new List<int>(list);
来源：http://daw.sufxvd.cn

[D23] reduce 累积计算
来源：http://kmi.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pnl.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bbv.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wpz.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbp.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://srk.shanyushiyangtech.top

Go:   // 手写循环
来源：http://cbk.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yjj.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dvp.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://hso.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rxi.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lcv.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rbd.pengpengdd.cyou

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://klp.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dvs.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ofi.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jkp.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://koc.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://nra.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fjg.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ckf.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://szb.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://euy.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dip.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zbs.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kbm.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dem.haohaochexian.top

[D26] 数组转字符串
来源：http://euy.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://cwi.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://fuw.yongpay.top

JS:   arr.join(", ")
来源：http://cue.vehdjk.com

TS:   arr.join(", ")
来源：http://jyp.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://fha.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://fgh.ydzc1.top

Ruby: arr.join(", ")
来源：http://ntz.smart0.xyz

C#:   string.Join(", ", list)
来源：http://uhs.shzxlz.cn

================================================================================
来源：http://tit.tianlin.xyz

E. 字符串处理
来源：http://zuo.gzhubu.top

================================================================================
来源：http://gbl.chenjidiqi.icu

[E01] 拼接字符串
来源：http://bpf.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qdl.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ccc.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ygu.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vfr.gogol.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qpv.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hri.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cvu.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ehg.zhijiandao.cn

[E02] 重复字符串
来源：http://ymn.kuanghao11.cn

Py:   "ab" * 3
来源：http://mzm.jinghuilouyu.cn

PHP:  str_repeat("ab", 3);
来源：http://kzq.daxiang520.top

JS:   "ab".repeat(3)
来源：http://myu.fzhhl.top

TS:   "ab".repeat(3)
来源：http://cnm.jiagoushi.top

Java: "ab".repeat(3)
来源：http://lyw.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://qam.smart0.xyz

Ruby: "ab" * 3
来源：http://pxb.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qne.yj20258888.top

[E03] 截取子串
来源：http://ajn.chenjidiqi.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nkd.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://owd.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mwv.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://bac.fengsongda.top

Java: s.substring(1, 4)
来源：http://mys.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://due.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://zxg.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://ynh.jianghu66.top

[E04] 查找子串位置
来源：http://qou.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://iby.yj20258.top

PHP:  strpos($s, "x");
来源：http://gzo.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://khg.ctjpmb.com

TS:   s.indexOf("x")
来源：http://kgo.jianghu66.top

Java: s.indexOf("x")
来源：http://iea.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://pgp.dashuyun.cn

Ruby: s.index("x")
来源：http://zxr.yvedp.cn

C#:   s.IndexOf("x")
来源：http://wye.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gor.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cea.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://esv.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lez.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xpf.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ken.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ioh.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jkd.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://idq.guowangkeji.top

[E06] 替换子串
来源：http://yas.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dbh.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://otp.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ipd.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://ybd.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vdw.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bny.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dhz.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://muj.andypj.xyz

[E07] 按分隔符拆分
来源：http://fop.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ggu.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qwi.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zmb.yuxming.cn

TS:   s.split(",")
来源：http://dny.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pfp.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://otj.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://uod.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nyp.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://kqv.cheryme.top

Py:   ",".join(items)
来源：http://tkc.daxiang520.top

PHP:  implode(",", $items);
来源：http://hgo.sxryk.cn

JS:   items.join(",")
来源：http://ddt.tianlin.xyz

TS:   items.join(",")
来源：http://rwa.yanxiufei.cn

Java: String.join(",", items)
来源：http://waa.tanke756.top

Go:   strings.Join(items, ",")
来源：http://faj.52xcode.cn

Ruby: items.join(",")
来源：http://oji.tian-w.cn

C#:   string.Join(",", items)
来源：http://wyl.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://sti.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kme.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zwt.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://nzb.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://vxl.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://zvs.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vaf.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://umj.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ths.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://nuo.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vfd.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nec.jqgfzy.top

JS:   "7".padStart(3, "0")
来源：http://pim.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://laz.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://grb.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mqv.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://slb.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sex.shzxlz.cn

[E11] 反转字符串
来源：http://zgg.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://dmt.zhiwuduotai.top

PHP:  strrev($s);
来源：http://sqo.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://zql.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://pso.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sql.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ojt.uphjek.com

Ruby: s.reverse
来源：http://apu.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://xus.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://yst.shangyingyoupin.top

Py:   s.count("a")
来源：http://lym.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://iyp.pycfn.com

JS:   s.split("a").length - 1
来源：http://xue.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://yxb.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fhb.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://bnh.gaohongyu789.top

Ruby: s.count("a")
来源：http://esa.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://vay.cdnleiting.top

[E13] 逐字符遍历
来源：http://iar.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://jzb.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qlg.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cdf.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oei.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cip.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kbc.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xvd.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://one.gzhubu.top

[E14] URL 编码与 Base64
来源：http://syw.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fnf.chenjidiqi.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://hxh.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xlu.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cvm.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uus.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dgd.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vef.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ruj.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://orp.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ylo.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mcu.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qyb.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://grk.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jix.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sxb.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://phm.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ona.bjfxy.top

[E16] 数字千分位
来源：http://uza.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://mwu.c1oappe.top

PHP:  number_format(1234567);
来源：http://xzc.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dwo.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://syn.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://psz.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dzi.zdbjq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iwy.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://roa.xylfe.cn

[E17] 首字母大写
来源：http://xiu.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vah.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lbs.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rmq.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qex.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aal.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zyw.sxryk.cn

Ruby: s.capitalize
来源：http://kgk.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://anj.yuxming.cn

[E18] 模板占位符替换
来源：http://yyd.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mxb.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aby.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tto.guannengcc.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cmd.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xuv.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kjk.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ziz.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xwq.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://srh.jianghu66.top

Py:   s.splitlines()
来源：http://nhu.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qwl.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://vpf.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://jas.gogol.net.cn

Java: s.lines().toList()
来源：http://vwg.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://ghb.ctjpmb.com

Ruby: s.lines
来源：http://qxr.hesvh.cn

C#:   s.Split('\n')
来源：http://xiv.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://bjk.jqgufenzy.top

Py:   if not s:
来源：http://dro.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zdh.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vrs.zhongyouzk.top

TS:   if (s === "") {}
来源：http://jvj.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://jga.jiagoushi.top

Go:   if s == "" {}
来源：http://kyh.shanyushiyangkeji.top

Ruby: if s.empty?
来源：http://nno.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zjq.shuidangran.top

[E21] 超长截断加省略号
来源：http://rge.hongshengwenyu.top


<!-- 参考信息 -->