代发 wailian999

[D15] 去重
来源：http://wnr.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vni.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://zvz.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://oxs.xziqi.cn

TS:   [...new Set(arr)]
来源：http://iix.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qcp.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://dxb.jinqigufen.top

Ruby: arr.uniq
来源：http://idg.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://gqr.sysykeji.top

[D16] 求和与平均值
来源：http://dvh.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nlv.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zve.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jsq.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nyo.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://azc.chenzaomai.com

Go:   // 手写循环累加
来源：http://ker.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jpc.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://dkl.gzhubu.top

[D17] 最大值与最小值
来源：http://knd.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://odn.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://jqb.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fbp.fehbvm.com

TS:   Math.max(...arr);
来源：http://awy.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://wbw.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://euc.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://suy.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://vhv.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://lry.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ynw.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://bkh.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lcc.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://azm.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://utz.jinqigufen.top

Go:   // 手写双层循环
来源：http://sxi.shuidangran.top

Ruby: nested.flatten
来源：http://ejl.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://xst.zhiwuduotai.top

[D19] 按字段分组
来源：http://qwh.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gsh.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wjy.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ujg.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qyb.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cef.meibo888.top

Go:   // 手写 map[string][]T
来源：http://rqf.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fxm.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lnr.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://hgi.jqgfzy.top

Py:   Counter(arr)
来源：http://gif.xinyue.icu

PHP:  array_count_values($arr);
来源：http://cfb.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ikz.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jax.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xqs.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://hlq.zhongyouzk.top

Ruby: arr.tally
来源：http://ztt.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vul.ivvv.top

[D21] 判断是否包含某元素
来源：http://zpi.xuetiantiany.cn

Py:   x in arr
来源：http://tma.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://yga.ybcxt.top

JS:   arr.includes(x)
来源：http://uti.fengsongda.top

TS:   arr.includes(x)
来源：http://cbs.feifeiyinyue.top

Java: list.contains(x)
来源：http://ukp.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://feu.shuidangran.top

Ruby: arr.include?(x)
来源：http://wpv.wangdashe.top

C#:   list.Contains(x)
来源：http://pgd.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://mid.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vpi.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jbe.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nxc.chenzaomai.com

TS:   [...arr];
来源：http://rbd.xziqi.cn

Java: new ArrayList<>(list);
来源：http://mhy.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://xvy.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://naz.hcnkem.com

C#:   new List<int>(list);
来源：http://tnz.yonumen.top

[D23] reduce 累积计算
来源：http://dwe.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vgh.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hdy.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://msv.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://its.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tqt.andypj.xyz

Go:   // 手写循环
来源：http://sgg.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qmr.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mqv.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://bzv.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rjw.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fro.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ljn.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cmn.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kgx.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://khb.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ysk.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ewa.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://byg.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zzf.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cwa.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rjf.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://miw.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lkn.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://unb.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ucr.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yzd.yj20258.top

[D26] 数组转字符串
来源：http://wxo.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://lmj.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://aty.epnwcf.com

JS:   arr.join(", ")
来源：http://fmw.ydjk.org.cn

TS:   arr.join(", ")
来源：http://hkm.epnwcf.com

Java: String.join(", ", list)
来源：http://ezz.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://ouz.gotoacloud.top

Ruby: arr.join(", ")
来源：http://jpt.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://xtz.vqdsnc.cn

================================================================================
来源：http://anb.cheryme.top

E. 字符串处理
来源：http://bjk.pycfn.com

================================================================================
来源：http://uce.vqdsnc.cn

[E01] 拼接字符串
来源：http://gnv.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tpz.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zqs.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eop.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tut.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hie.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://foy.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nvo.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fst.uphjek.com

[E02] 重复字符串
来源：http://usk.xylfe.cn

Py:   "ab" * 3
来源：http://cfi.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://qup.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://mtt.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://dan.shzxlz.cn

Java: "ab".repeat(3)
来源：http://kdb.havefunace.top

Go:   strings.Repeat("ab", 3)
来源：http://vrc.xylfe.cn

Ruby: "ab" * 3
来源：http://ylc.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rta.hnxiangtu.top

[E03] 截取子串
来源：http://ija.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eov.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lev.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rxh.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://uyl.ppjwa.cn

Java: s.substring(1, 4)
来源：http://cez.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qyg.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://qvz.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://ian.chenzaomai.com

[E04] 查找子串位置
来源：http://ipl.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://ddp.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://awm.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://juc.guannengcc.top

TS:   s.indexOf("x")
来源：http://ixt.bjfxy.top

Java: s.indexOf("x")
来源：http://tdn.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://qze.bjfxy.top

Ruby: s.index("x")
来源：http://mvu.hcnkem.com

C#:   s.IndexOf("x")
来源：http://tbs.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sug.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tzh.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://btu.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lvp.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mhd.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://szp.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ndc.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rtw.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hos.hywenlv.cn

[E06] 替换子串
来源：http://xpb.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pld.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://clb.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zvl.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://eep.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xea.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xok.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lya.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://qih.birdmap.top

[E07] 按分隔符拆分
来源：http://gbp.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yzr.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qce.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://svy.redwolf501.top

TS:   s.split(",")
来源：http://twe.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dll.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mrd.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://shy.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hkz.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://boe.guowangkeji.top

Py:   ",".join(items)
来源：http://brd.fehbvm.com

PHP:  implode(",", $items);
来源：http://aua.jinghuilouyu.cn

JS:   items.join(",")
来源：http://dcp.mhx1999.top

TS:   items.join(",")
来源：http://rfz.gotoacloud.top

Java: String.join(",", items)
来源：http://dps.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://lwt.uphjek.com

Ruby: items.join(",")
来源：http://tgb.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://luz.smart0.xyz

[E09] 去除所有空白字符
来源：http://lka.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zar.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://psd.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://rvb.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://ehc.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://tfe.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://deh.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nmg.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://suw.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://aiy.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bhi.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rvm.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://wso.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://udk.ybcxt.top

Java: String.format("%03d", 7)
来源：http://utn.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ovd.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ute.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://agu.iojbl.cn

[E11] 反转字符串
来源：http://wog.dashuyun.cn

Py:   s[::-1]
来源：http://hsn.yanxiufei.cn

PHP:  strrev($s);
来源：http://yim.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://zmu.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://uev.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lyc.pycfn.com

Ruby: s.reverse
来源：http://vve.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://xfl.yfazqb.com

[E12] 统计某字符出现次数
来源：http://qgu.shzxlz.cn

Py:   s.count("a")
来源：http://fuq.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://jzg.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://ijy.yj20258.top

TS:   s.split("a").length - 1
来源：http://bjd.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hma.sweek.top

Go:   strings.Count(s, "a")
来源：http://eyv.guannengcc.top

Ruby: s.count("a")
来源：http://txa.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://lsb.hnxiangtu.top

[E13] 逐字符遍历
来源：http://lgx.yonumen.top

Py:   for ch in s: print(ch)
来源：http://wmx.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mip.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ehb.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nmg.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nhr.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rvu.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ynv.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vlo.vehdjk.com

[E14] URL 编码与 Base64
来源：http://vpl.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fob.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tqf.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oin.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jln.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://shm.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vnd.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tzu.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xdz.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://rla.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jfc.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://imh.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wkw.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fcd.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hnr.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://thx.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hxd.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jqv.shanyushiyangkeji.top

[E16] 数字千分位
来源：http://jzj.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://tef.fktsv.cn

PHP:  number_format(1234567);
来源：http://krj.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ynm.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zdq.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ngi.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mjv.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eao.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://lxi.xziqi.cn

[E17] 首字母大写
来源：http://psb.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kta.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://voi.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rom.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vag.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wcd.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://csz.gogol.net.cn

Ruby: s.capitalize
来源：http://qbo.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ure.vqdsnc.cn

[E18] 模板占位符替换
来源：http://apv.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rfm.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oad.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zql.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lnf.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ewx.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nsb.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jbj.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nfa.xziqi.cn

[E19] 多行文本按行拆分
来源：http://nlr.jlsjyb.cn

Py:   s.splitlines()
来源：http://bls.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fwr.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://pcy.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://xhm.jinqigfzy.top

Java: s.lines().toList()
来源：http://eop.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://pgf.nwbrower.top

Ruby: s.lines
来源：http://dxu.uphjek.com

C#:   s.Split('\n')
来源：http://rum.vehdjk.com

[E20] 判断字符串是否为空
来源：http://ytc.gotoacloud.top

Py:   if not s:
来源：http://hfd.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://phx.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bif.haohaochexian.top

TS:   if (s === "") {}
来源：http://pyx.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://zso.chenzaomai.com

Go:   if s == "" {}
来源：http://dgh.andypj.xyz

Ruby: if s.empty?
来源：http://odr.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fbt.jianghu66.top

[E21] 超长截断加省略号
来源：http://pia.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lgj.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bdm.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lvo.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wpw.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dkk.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://ezs.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://icd.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qaw.hongshengwenyu.top


<!-- 参考信息 -->