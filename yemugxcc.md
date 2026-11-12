代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vwk.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sxc.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://cbs.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://qun.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gwj.sjlbkw.cn

Go:   // 手写循环
来源：http://dmd.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://nbk.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rgo.zhoulong.xyz

[D15] 去重
来源：http://ohg.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zdl.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://zpj.gzhubu.top

JS:   [...new Set(arr)]
来源：http://lfz.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://ofc.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oez.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qwc.epnwcf.com

Ruby: arr.uniq
来源：http://ipy.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://phl.c1oappe.top

[D16] 求和与平均值
来源：http://iot.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://emz.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dpx.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ech.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cjg.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ufi.yonumen.top

Go:   // 手写循环累加
来源：http://wfd.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ncm.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://lnp.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://ram.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://ytd.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://vui.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://con.yvedp.cn

TS:   Math.max(...arr);
来源：http://sll.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fti.sysykeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cjb.cheryme.top

Ruby: arr.max;  arr.min
来源：http://qth.yj20258.top

C#:   list.Max();  list.Min()
来源：http://eko.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://anx.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ejv.yj20258.top

PHP:  array_merge(...$nested);
来源：http://ruy.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ezr.yangfankeji.com

TS:   nested.flat();
来源：http://owx.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://asd.uphjek.com

Go:   // 手写双层循环
来源：http://qxj.zycfv.cn

Ruby: nested.flatten
来源：http://owu.hcnkem.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://sai.nwbrower.top

[D19] 按字段分组
来源：http://eyq.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cxn.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kqk.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ohv.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mdm.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fpj.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://soo.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xvs.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://drf.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://awb.yuxming.cn

Py:   Counter(arr)
来源：http://jxr.yfazqb.com

PHP:  array_count_values($arr);
来源：http://fcq.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://taj.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gkx.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qri.hesvh.cn

Go:   // 手写 map[T]int
来源：http://ijd.havefunace.top

Ruby: arr.tally
来源：http://lbd.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yag.fengsongda.top

[D21] 判断是否包含某元素
来源：http://pht.hfpthk.cn

Py:   x in arr
来源：http://nfg.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://qaa.daria6918.cn

JS:   arr.includes(x)
来源：http://ipj.wangdashe.top

TS:   arr.includes(x)
来源：http://skx.jqgufenzy.top

Java: list.contains(x)
来源：http://odw.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://fzg.ybcxt.top

Ruby: arr.include?(x)
来源：http://vlw.tarul.cn

C#:   list.Contains(x)
来源：http://dml.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://alh.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fsl.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qco.snrcjt.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://owa.xuetiantiany.cn

TS:   [...arr];
来源：http://qyn.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://oju.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nhj.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://lux.vqdsnc.cn

C#:   new List<int>(list);
来源：http://niz.svipenyu.cn

[D23] reduce 累积计算
来源：http://klm.iojbl.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yby.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wwb.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ceh.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lkp.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ovz.yj202588.top

Go:   // 手写循环
来源：http://det.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://thi.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fup.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://nak.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zrj.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bbt.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ztg.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rtz.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aup.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bdh.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://teq.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mxr.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://nib.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lgt.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vnm.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dmy.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yjr.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tin.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://npc.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ald.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ppu.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://xyo.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://jdu.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://xwp.dianchejie.cn

JS:   arr.join(", ")
来源：http://oix.tanke756.top

TS:   arr.join(", ")
来源：http://kxs.hnxiangtu.top

Java: String.join(", ", list)
来源：http://ads.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://ktv.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://ane.fzhhl.top

C#:   string.Join(", ", list)
来源：http://zno.c1oappe.top

================================================================================
来源：http://gzq.svipenyu.cn

E. 字符串处理
来源：http://jvl.chenzaomai.com

================================================================================
来源：http://afi.kuanghao11.cn

[E01] 拼接字符串
来源：http://roj.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zis.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oyu.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://onm.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iff.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gyo.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xge.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://axa.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jwp.sufxvd.cn

[E02] 重复字符串
来源：http://sme.jianghu66.top

Py:   "ab" * 3
来源：http://ofk.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://ulp.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://yvo.fzhhl.top

TS:   "ab".repeat(3)
来源：http://apm.wangdashe.top

Java: "ab".repeat(3)
来源：http://mif.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://mjz.ybcxt.top

Ruby: "ab" * 3
来源：http://sbn.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cel.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://mzb.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rcu.yvedp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eqo.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://thb.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://lmi.dianchejie.cn

Java: s.substring(1, 4)
来源：http://prg.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pox.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://rpf.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://tda.c1oappe.top

[E04] 查找子串位置
来源：http://oio.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://yki.jlsjyb.cn

PHP:  strpos($s, "x");
来源：http://avv.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rlg.ctjpmb.com

TS:   s.indexOf("x")
来源：http://tho.bbcook.cn

Java: s.indexOf("x")
来源：http://kkc.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://reo.yanxiufei.cn

Ruby: s.index("x")
来源：http://uja.iojbl.cn

C#:   s.IndexOf("x")
来源：http://flk.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://klw.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ysl.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zop.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gib.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://rby.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wer.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mnq.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mqe.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ihr.cucudq.cn

[E06] 替换子串
来源：http://apw.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://epv.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://vzc.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gdo.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://bfe.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hbt.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nxx.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tts.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://ujb.sxryk.cn

[E07] 按分隔符拆分
来源：http://lcn.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pou.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fhy.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ltr.ydjk.org.cn

TS:   s.split(",")
来源：http://iam.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://alk.ehwqpu.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ewk.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://gjc.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dxw.havefunace.top

[E08] 数组按分隔符合并
来源：http://wjx.gogol.net.cn

Py:   ",".join(items)
来源：http://tdl.yuxming.cn

PHP:  implode(",", $items);
来源：http://kqa.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://pbg.fzhhl.top

TS:   items.join(",")
来源：http://goc.cheryme.top

Java: String.join(",", items)
来源：http://lhn.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://eax.smart0.xyz

Ruby: items.join(",")
来源：http://bmc.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://xjf.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://phn.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://onz.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ory.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://mwk.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://mwv.cucudq.cn

Java: s.replaceAll("\\s+", "")
来源：http://hzd.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ctf.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sem.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dpz.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://dsg.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sjj.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://izl.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://hka.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://kaf.zycfv.cn

Java: String.format("%03d", 7)
来源：http://zec.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cjo.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yhz.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://enq.iojbl.cn

[E11] 反转字符串
来源：http://azb.wangdashe.top

Py:   s[::-1]
来源：http://ipc.ctjpmb.com

PHP:  strrev($s);
来源：http://lye.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://wdl.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://uuv.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ooc.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mxe.dianchejie.cn

Ruby: s.reverse
来源：http://ewh.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oct.jianghu66.top

[E12] 统计某字符出现次数
来源：http://yji.aizwys.cn

Py:   s.count("a")
来源：http://dml.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://ywu.tanke756.top

JS:   s.split("a").length - 1
来源：http://ciy.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://mbp.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xau.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://rxv.vqdsnc.cn

Ruby: s.count("a")
来源：http://jkd.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://mgs.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://yit.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://yrt.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://esj.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qwk.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hfc.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lug.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fya.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tzx.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aap.hammf.cn

[E14] URL 编码与 Base64
来源：http://uhc.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dhy.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ceq.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iiz.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sce.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://slq.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gyy.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kok.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eol.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://qfs.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ouy.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ukz.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lqw.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qyw.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zaz.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nzm.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vdw.dashuyun.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gvh.sweek.top

[E16] 数字千分位
来源：http://jmr.xylfe.cn

Py:   f"{1234567:,}"
来源：http://ofm.jinqigufen.top

PHP:  number_format(1234567);
来源：http://qct.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://umf.tian-w.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://svd.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://muf.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oxa.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tym.yfazqb.com

C#:   1234567.ToString("N0")
来源：http://lgb.svipenyu.cn

[E17] 首字母大写
来源：http://nsn.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fwp.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rrb.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cjg.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ble.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jys.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://imx.jiagoushi.top

Ruby: s.capitalize
来源：http://qhc.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zuw.yanxiufei.cn

[E18] 模板占位符替换
来源：http://rei.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jja.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fkf.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dow.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ukd.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://prt.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hld.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bmz.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otf.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://yyv.yj202588.top

Py:   s.splitlines()
来源：http://ois.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tsb.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://acf.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://xnq.daria6918.cn

Java: s.lines().toList()
来源：http://bly.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://poe.mhx1999.top

Ruby: s.lines
来源：http://bms.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://yac.guannengcc.top

[E20] 判断字符串是否为空
来源：http://ont.yuanzhike.top

Py:   if not s:
来源：http://apa.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xie.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yjy.shzxlz.cn

TS:   if (s === "") {}
来源：http://gps.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://idj.daxiang520.top

Go:   if s == "" {}
来源：http://gxc.zhijiandao.cn

Ruby: if s.empty?
来源：http://lwd.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lqr.fengsongda.top

[E21] 超长截断加省略号
来源：http://hgt.zycfv.cn


<!-- 参考信息 -->