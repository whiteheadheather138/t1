代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://qvf.svipenyu.cn

Go:   // 手写循环
来源：http://xmc.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://rhc.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xpm.jiagoushi.top

[D15] 去重
来源：http://crw.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cnu.gogol.net.cn

PHP:  array_unique($arr);
来源：http://ufp.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://xkz.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://scr.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ujt.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vvq.haohaochexian.top

Ruby: arr.uniq
来源：http://bou.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://ifu.zdbjq.cn

[D16] 求和与平均值
来源：http://wil.xuanzx.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hbj.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yqu.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wjv.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vkb.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wwe.shzxlz.cn

Go:   // 手写循环累加
来源：http://aij.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bdn.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://ecd.zycfv.cn

[D17] 最大值与最小值
来源：http://fbv.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://igw.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://dcw.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pno.daxiang520.top

TS:   Math.max(...arr);
来源：http://pmg.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lrj.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ovv.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://clr.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://gwg.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://otr.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rdv.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://yui.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://omo.ybcxt.top

TS:   nested.flat();
来源：http://vqx.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://buf.dianchejie.cn

Go:   // 手写双层循环
来源：http://daz.cashguo.top

Ruby: nested.flatten
来源：http://eog.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://jte.fehbvm.com

[D19] 按字段分组
来源：http://awa.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vcv.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://izg.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ika.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lcu.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fyw.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://wbc.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gwv.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jnn.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://nxt.snrcjt.cn

Py:   Counter(arr)
来源：http://uly.yueranfly.top

PHP:  array_count_values($arr);
来源：http://lxg.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyf.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vgf.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cfo.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://ihc.hammf.cn

Ruby: arr.tally
来源：http://ott.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dgn.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://wom.nanxinkj.top

Py:   x in arr
来源：http://ybw.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://utz.hnxiangtu.top

JS:   arr.includes(x)
来源：http://vss.yfazqb.com

TS:   arr.includes(x)
来源：http://zpz.tanke756.top

Java: list.contains(x)
来源：http://qyo.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://tey.shzxlz.cn

Ruby: arr.include?(x)
来源：http://znh.yfazqb.com

C#:   list.Contains(x)
来源：http://emx.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://ccs.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nua.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xnj.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fsq.sxryk.cn

TS:   [...arr];
来源：http://jvl.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://wyb.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bsm.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://ara.hfpthk.cn

C#:   new List<int>(list);
来源：http://sia.yongpay.top

[D23] reduce 累积计算
来源：http://yic.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xmr.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wkg.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kno.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vsz.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rfe.jinqigufen.top

Go:   // 手写循环
来源：http://jgg.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zih.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ngs.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://jtf.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sau.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rik.cucudq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xde.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gam.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fku.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hlo.hesvh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wpv.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ztu.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://spk.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tak.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kqo.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://epb.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xdi.jianghu66.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vax.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pnm.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://srq.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bcn.fengsongda.top

[D26] 数组转字符串
来源：http://wdw.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://eaz.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://qca.zycfv.cn

JS:   arr.join(", ")
来源：http://eca.jlsjyb.cn

TS:   arr.join(", ")
来源：http://cdo.hnxiangtu.top

Java: String.join(", ", list)
来源：http://qpz.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://dgv.ppjwa.cn

Ruby: arr.join(", ")
来源：http://hfb.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://srw.ppjwa.cn

================================================================================
来源：http://osg.yvedp.cn

E. 字符串处理
来源：http://vbq.wangshuangyany.cn

================================================================================
来源：http://rsd.hnqzz.top

[E01] 拼接字符串
来源：http://cnt.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hka.haohaochexian.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xvb.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cwa.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hhx.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://swj.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://axy.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ktu.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vqi.zycfv.cn

[E02] 重复字符串
来源：http://jim.zhixingplan.top

Py:   "ab" * 3
来源：http://biv.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://dah.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://ulw.iojbl.cn

TS:   "ab".repeat(3)
来源：http://sux.jianghu66.top

Java: "ab".repeat(3)
来源：http://xsp.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://tbm.yongpay.top

Ruby: "ab" * 3
来源：http://xej.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://brs.ybcxt.top

[E03] 截取子串
来源：http://zhh.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ezf.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sor.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://noc.hcnkem.com

TS:   s.slice(1, 4)
来源：http://ykj.sysykeji.top

Java: s.substring(1, 4)
来源：http://gjx.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://udu.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://omu.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://ytx.xziqi.cn

[E04] 查找子串位置
来源：http://bff.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://gdu.yongpay.top

PHP:  strpos($s, "x");
来源：http://pwk.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kga.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://obn.mhx1999.top

Java: s.indexOf("x")
来源：http://cqc.cheryme.top

Go:   strings.Index(s, "x")
来源：http://pkv.hnxiangtu.top

Ruby: s.index("x")
来源：http://rso.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://tpb.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zsf.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cgz.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ipb.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hja.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oar.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qiv.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kqw.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ylu.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://byc.cdnleiting.top

[E06] 替换子串
来源：http://rod.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kps.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://gxy.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjq.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://fks.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://huj.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zvo.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mvv.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://glp.daria6918.cn

[E07] 按分隔符拆分
来源：http://kyb.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gqb.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ipo.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eaf.vqdsnc.cn

TS:   s.split(",")
来源：http://vht.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vvu.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bwj.pycfn.com

Ruby: s.split(",");  s.split
来源：http://cpq.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mff.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://jev.cqqwz.cn

Py:   ",".join(items)
来源：http://zqm.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://jjf.zhixingplan.top

JS:   items.join(",")
来源：http://deq.xylfe.cn

TS:   items.join(",")
来源：http://ygx.hnqzz.top

Java: String.join(",", items)
来源：http://jsi.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://uml.andypj.xyz

Ruby: items.join(",")
来源：http://kis.yj202588.top

C#:   string.Join(",", items)
来源：http://grh.yfazqb.com

[E09] 去除所有空白字符
来源：http://ibg.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rgw.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uko.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://vic.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://hgy.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://pxj.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xzz.kuanghao11.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mhs.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://drv.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://sxs.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mzg.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hmv.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://viy.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://iup.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://xpx.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://frx.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://znv.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://smk.uphjek.com

[E11] 反转字符串
来源：http://xwe.chenzaomai.com

Py:   s[::-1]
来源：http://ewo.xziqi.cn

PHP:  strrev($s);
来源：http://sbj.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://etl.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://dce.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ljp.yuxming.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rlc.yfazqb.com

Ruby: s.reverse
来源：http://fuo.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://yah.tanke756.top

[E12] 统计某字符出现次数
来源：http://kjg.redwolf501.top

Py:   s.count("a")
来源：http://klm.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://pdn.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://tnm.wangdashe.top

TS:   s.split("a").length - 1
来源：http://pbb.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yjw.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://iih.birdmap.top

Ruby: s.count("a")
来源：http://bpw.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://cmp.yvedp.cn

[E13] 逐字符遍历
来源：http://xue.birdmap.top

Py:   for ch in s: print(ch)
来源：http://drq.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ruj.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sxk.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://njw.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eyw.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oea.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mjy.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kwp.hesvh.cn

[E14] URL 编码与 Base64
来源：http://ozv.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vwn.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pbh.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ngt.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eci.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lol.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zej.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lfm.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aff.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://oot.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ypa.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://szj.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pow.ydjk.org.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://crv.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pog.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hxl.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gsr.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://irz.yvedp.cn

[E16] 数字千分位
来源：http://awo.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://nwg.cashguo.top

PHP:  number_format(1234567);
来源：http://qkz.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oni.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tdj.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ciq.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ine.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tki.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://ayj.shuidangran.top

[E17] 首字母大写
来源：http://mvz.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rql.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://eqa.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rvx.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pua.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uyf.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ipn.xylfe.cn

Ruby: s.capitalize
来源：http://sth.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pvu.haohaochexian.top

[E18] 模板占位符替换
来源：http://uxc.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sgq.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gjz.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://nxf.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zwk.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cal.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zfk.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bsx.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jwl.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://zwe.sufxvd.cn

Py:   s.splitlines()
来源：http://gap.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vwo.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://fsh.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://ity.yj202588.top

Java: s.lines().toList()
来源：http://rwo.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://wjx.yj20258.top

Ruby: s.lines
来源：http://out.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://dpj.aizwys.cn

[E20] 判断字符串是否为空
来源：http://zqg.yj20258888.top

Py:   if not s:
来源：http://xoa.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qid.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hjy.tarul.cn

TS:   if (s === "") {}
来源：http://jpu.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://uyy.xziqi.cn

Go:   if s == "" {}
来源：http://jli.cheryme.top

Ruby: if s.empty?
来源：http://qnn.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ouf.c1oappe.top

[E21] 超长截断加省略号
来源：http://zuc.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rhh.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tgf.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ppv.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dco.yj20258.top


<!-- 参考信息 -->