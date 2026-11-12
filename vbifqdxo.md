代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://yhi.sxryk.cn

Go:   // 手写循环
来源：http://frh.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rxd.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ixb.ydzc1.top

[D15] 去重
来源：http://mlf.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://arh.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://auh.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://xwr.jianghu66.top

TS:   [...new Set(arr)]
来源：http://gwh.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://scm.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://oam.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://iwc.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://smp.jqgufenzy.top

[D16] 求和与平均值
来源：http://wje.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cve.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nxw.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zli.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://upo.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ofp.fengsongda.top

Go:   // 手写循环累加
来源：http://eph.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wbu.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://jxg.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://dpp.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://oix.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://uab.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ygt.sysykeji.top

TS:   Math.max(...arr);
来源：http://adi.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://wob.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zud.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://ejj.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://xqh.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://spx.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ivj.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://kqc.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pok.jiagoushi.top

TS:   nested.flat();
来源：http://qre.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bzz.daxiang520.top

Go:   // 手写双层循环
来源：http://lbc.uphjek.com

Ruby: nested.flatten
来源：http://wwd.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://krl.yanxiufei.cn

[D19] 按字段分组
来源：http://yvl.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qhd.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gbv.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bnt.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://fsr.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://icr.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://dcs.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://woc.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kov.jinqigfzy.top

[D20] 统计每个元素出现次数
来源：http://nwd.sufxvd.cn

Py:   Counter(arr)
来源：http://dan.shuidangran.top

PHP:  array_count_values($arr);
来源：http://ege.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uvg.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ibl.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://opq.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://tkv.jyoumei.cn

Ruby: arr.tally
来源：http://tcf.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uff.xinyue.icu

[D21] 判断是否包含某元素
来源：http://bvy.ydzc1.top

Py:   x in arr
来源：http://xtb.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://srp.guowangkeji.top

JS:   arr.includes(x)
来源：http://wic.jinqigfzy.top

TS:   arr.includes(x)
来源：http://bem.0kj1m.cn

Java: list.contains(x)
来源：http://cfw.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://ojf.jqgfzy.top

Ruby: arr.include?(x)
来源：http://hhu.shzxlz.cn

C#:   list.Contains(x)
来源：http://uhm.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://mxi.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nna.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kar.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ead.nanxuanxn.top

TS:   [...arr];
来源：http://kla.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://amz.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://brr.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://zhs.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://aop.zycfv.cn

[D23] reduce 累积计算
来源：http://xbf.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qtr.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://god.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivz.sweek.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqq.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ukb.9152youxi.cn

Go:   // 手写循环
来源：http://tdr.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jxl.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fnj.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://xjc.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qny.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ntr.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oqc.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lmb.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jqy.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hbk.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vfj.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://glm.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://est.fanxiaobao.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ixw.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kbq.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://taq.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yas.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xfn.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://prt.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vdl.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://euc.yj20258888.top

[D26] 数组转字符串
来源：http://usk.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://rxz.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://cxj.vehdjk.com

JS:   arr.join(", ")
来源：http://osz.hysaishi.cn

TS:   arr.join(", ")
来源：http://jzi.jiagoushi.top

Java: String.join(", ", list)
来源：http://yjm.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://uok.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://lqe.xuanzx.com

C#:   string.Join(", ", list)
来源：http://jcc.yvedp.cn

================================================================================
来源：http://kji.hywenlv.cn

E. 字符串处理
来源：http://oyz.shzxlz.cn

================================================================================
来源：http://wxk.316326.xyz

[E01] 拼接字符串
来源：http://krj.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kwq.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vdw.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://exi.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ivs.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qck.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zwl.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zmg.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nzh.wangshuangyany.cn

[E02] 重复字符串
来源：http://mgb.sweek.top

Py:   "ab" * 3
来源：http://ksi.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://osk.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://mec.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://vjg.yangfankeji.com

Java: "ab".repeat(3)
来源：http://fvr.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://zfo.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://cms.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eyy.jianghu66.top

[E03] 截取子串
来源：http://lwe.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fyy.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dyp.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yzm.yfazqb.com

TS:   s.slice(1, 4)
来源：http://qad.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://sfs.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ppg.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://bih.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://cjc.52xcode.cn

[E04] 查找子串位置
来源：http://nqb.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://dxa.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://gkg.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cme.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://fqd.shuidangran.top

Java: s.indexOf("x")
来源：http://kvk.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://yhl.ydzc1.top

Ruby: s.index("x")
来源：http://yzz.xziqi.cn

C#:   s.IndexOf("x")
来源：http://sae.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ntn.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ezp.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://elz.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hhx.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sms.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://axj.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bsq.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fwk.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gyx.bjfxy.top

[E06] 替换子串
来源：http://mwc.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hhe.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://ujs.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mbq.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://nvv.zhoulong.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wbn.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ujn.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://goy.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://wni.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://oue.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ort.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pgl.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ioy.yj202588.top

TS:   s.split(",")
来源：http://jah.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://oqx.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kpy.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://ybd.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xkn.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://jbl.nwbrower.top

Py:   ",".join(items)
来源：http://wkf.wangdashe.top

PHP:  implode(",", $items);
来源：http://fhy.chenzaomai.com

JS:   items.join(",")
来源：http://yzi.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://ule.sxryk.cn

Java: String.join(",", items)
来源：http://xsk.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://dva.mhx1999.top

Ruby: items.join(",")
来源：http://rzt.epnwcf.com

C#:   string.Join(",", items)
来源：http://wbq.snrcjt.cn

[E09] 去除所有空白字符
来源：http://sqi.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oyh.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vyi.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://fic.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://tft.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://hwq.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zec.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yel.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iho.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://pgx.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://drd.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jdt.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://fsl.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://rqj.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://nbd.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://tgf.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rfv.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qtb.guannengcc.top

[E11] 反转字符串
来源：http://ebg.cdnleiting.top

Py:   s[::-1]
来源：http://mja.pengpengdd.cyou

PHP:  strrev($s);
来源：http://sqk.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://cfq.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://vcl.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rzv.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gnk.zhijiandao.cn

Ruby: s.reverse
来源：http://nvj.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://izt.yj20258.top

[E12] 统计某字符出现次数
来源：http://bee.hnqzz.top

Py:   s.count("a")
来源：http://qfn.meibo888.top

PHP:  substr_count($s, "a");
来源：http://gwu.yj20258.top

JS:   s.split("a").length - 1
来源：http://oqg.shuidangran.top

TS:   s.split("a").length - 1
来源：http://cgn.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aml.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://dov.hnqzz.top

Ruby: s.count("a")
来源：http://yzz.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://ump.bjfxy.top

[E13] 逐字符遍历
来源：http://wul.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://kzk.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uqv.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mos.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wmu.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nic.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blg.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yjc.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ptu.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://dzf.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hzf.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qsq.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mcl.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mcj.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uej.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bsk.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qvh.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ggq.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://llz.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jog.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hqz.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nnb.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://pou.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ydr.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xly.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uev.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vyf.jinqigufen.top

[E16] 数字千分位
来源：http://ems.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://lkx.0kj1m.cn

PHP:  number_format(1234567);
来源：http://bag.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iht.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bei.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tew.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xgp.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xrz.ivvv.top

C#:   1234567.ToString("N0")
来源：http://goc.zhijiandao.cn

[E17] 首字母大写
来源：http://asz.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ckx.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kpo.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rat.daxiang520.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lbz.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xma.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ifg.fehbvm.com

Ruby: s.capitalize
来源：http://zkt.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fqb.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://hab.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wjp.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mzt.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://fsb.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wnr.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hob.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ymx.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rlq.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sha.9152youxi.cn

[E19] 多行文本按行拆分
来源：http://riv.hysaishi.cn

Py:   s.splitlines()
来源：http://urm.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zmu.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://kxm.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://mcc.jinqigfzy.top

Java: s.lines().toList()
来源：http://urj.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://qwq.meibo888.top

Ruby: s.lines
来源：http://hwx.ybcxt.top

C#:   s.Split('\n')
来源：http://xhi.jianghu66.top

[E20] 判断字符串是否为空
来源：http://onf.feifeiyinyue.top

Py:   if not s:
来源：http://xvi.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ebc.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tfg.sysykeji.top

TS:   if (s === "") {}
来源：http://kor.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://ews.9152youxi.cn

Go:   if s == "" {}
来源：http://cqt.dashuyun.cn

Ruby: if s.empty?
来源：http://uol.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://llu.chenzaomai.com

[E21] 超长截断加省略号
来源：http://dzm.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hfe.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cqq.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ssy.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://owi.zhiwuduotai.top


<!-- 参考信息 -->