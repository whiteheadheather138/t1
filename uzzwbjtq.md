代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pcw.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gnf.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://rgb.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://jaz.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uyq.316326.xyz

Go:   // 手写循环
来源：http://fnv.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://lcz.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kgq.bbcook.cn

[D15] 去重
来源：http://mrw.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vvl.gotoacloud.top

PHP:  array_unique($arr);
来源：http://sjy.epnwcf.com

JS:   [...new Set(arr)]
来源：http://wbg.yuxming.cn

TS:   [...new Set(arr)]
来源：http://nkh.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ezm.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://ldt.fzhhl.top

Ruby: arr.uniq
来源：http://txc.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://spt.jiagoushi.top

[D16] 求和与平均值
来源：http://ftt.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xqz.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jpj.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aox.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://abx.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ord.uphjek.com

Go:   // 手写循环累加
来源：http://fab.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dto.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://vjm.jqgufenzy.top

[D17] 最大值与最小值
来源：http://jfz.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://iia.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://omq.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yuu.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://dzk.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rjt.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eka.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://rmi.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://pbs.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://dgp.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mjr.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://tgv.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://afa.chenzaomai.com

TS:   nested.flat();
来源：http://nzn.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hen.zhijiandao.cn

Go:   // 手写双层循环
来源：http://apm.jqgfzy.top

Ruby: nested.flatten
来源：http://sgw.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yuc.sxryk.cn

[D19] 按字段分组
来源：http://vkq.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sgc.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hvd.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uyp.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://blw.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://klg.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://xlf.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xtu.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yas.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://ssv.snrcjt.cn

Py:   Counter(arr)
来源：http://nxi.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://zoz.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rwa.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://keg.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zig.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://bbc.dashuyun.cn

Ruby: arr.tally
来源：http://bqm.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vei.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://iaw.yangfankeji.com

Py:   x in arr
来源：http://ayy.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://hij.hammf.cn

JS:   arr.includes(x)
来源：http://brn.fktsv.cn

TS:   arr.includes(x)
来源：http://mmz.ivvv.top

Java: list.contains(x)
来源：http://zpa.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://zoc.yj20258888.top

Ruby: arr.include?(x)
来源：http://fyg.zhengqikj.top

C#:   list.Contains(x)
来源：http://ckg.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://gmq.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ajz.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bpk.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://evz.wangdashe.top

TS:   [...arr];
来源：http://gry.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://doq.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://qzn.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://ehi.fktsv.cn

C#:   new List<int>(list);
来源：http://cqp.52xcode.cn

[D23] reduce 累积计算
来源：http://nxo.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gvi.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sbf.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lff.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hkb.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fff.havefunace.top

Go:   // 手写循环
来源：http://prq.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zee.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lsl.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://hka.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hiy.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zrz.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qcy.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lvt.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://toq.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sin.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bfu.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://diu.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://wqt.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://edn.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bqv.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jgf.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ibk.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fbz.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://opo.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cvh.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xrc.xuanzx.com

[D26] 数组转字符串
来源：http://cnb.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://qdy.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://jrt.cashguo.top

JS:   arr.join(", ")
来源：http://hio.52xcode.cn

TS:   arr.join(", ")
来源：http://dyg.yuanzhike.top

Java: String.join(", ", list)
来源：http://kub.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://egv.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://gld.andypj.xyz

C#:   string.Join(", ", list)
来源：http://znx.hcnkem.com

================================================================================
来源：http://hnw.cdnleiting.top

E. 字符串处理
来源：http://jvq.fanxiaobao.xyz

================================================================================
来源：http://ucx.nanxuanxn.top

[E01] 拼接字符串
来源：http://yhw.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ute.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vgk.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lbx.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://guh.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tdt.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rcg.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fiq.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bdc.sweek.top

[E02] 重复字符串
来源：http://asg.fzhhl.top

Py:   "ab" * 3
来源：http://kur.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://rit.zhijiandao.cn

JS:   "ab".repeat(3)
来源：http://wdr.hcnkem.com

TS:   "ab".repeat(3)
来源：http://dby.fehbvm.com

Java: "ab".repeat(3)
来源：http://upa.jiagoushi.top

Go:   strings.Repeat("ab", 3)
来源：http://hxj.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://tdc.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rva.shuidangran.top

[E03] 截取子串
来源：http://cye.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ewd.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tim.fanxiaobao.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dyw.yongpay.top

TS:   s.slice(1, 4)
来源：http://fmm.zdbjq.cn

Java: s.substring(1, 4)
来源：http://bbp.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://raj.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://zbd.uphjek.com

C#:   s.Substring(1, 3)
来源：http://oop.zhijiandao.cn

[E04] 查找子串位置
来源：http://mdo.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://wos.tian-w.cn

PHP:  strpos($s, "x");
来源：http://xph.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hpl.jyoumei.cn

TS:   s.indexOf("x")
来源：http://sut.haohaochexian.top

Java: s.indexOf("x")
来源：http://gvq.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://ply.zdqjudy.top

Ruby: s.index("x")
来源：http://uqq.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://noh.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mly.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fdv.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iti.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zwa.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qte.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wvr.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qid.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pll.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zjn.chenlongwang.top

[E06] 替换子串
来源：http://vwe.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ubg.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://bxb.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gcd.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://vys.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://umh.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cxv.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vxk.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://uja.iojbl.cn

[E07] 按分隔符拆分
来源：http://mpe.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gav.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kud.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fel.daxiang520.top

TS:   s.split(",")
来源：http://uvv.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://gld.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ddi.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://una.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://avg.sxryk.cn

[E08] 数组按分隔符合并
来源：http://wpp.yanxiufei.cn

Py:   ",".join(items)
来源：http://gfj.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://jvn.xylfe.cn

JS:   items.join(",")
来源：http://nng.zycfv.cn

TS:   items.join(",")
来源：http://mxx.hnxiangtu.top

Java: String.join(",", items)
来源：http://fzs.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://utn.iojbl.cn

Ruby: items.join(",")
来源：http://uzb.zdbjq.cn

C#:   string.Join(",", items)
来源：http://uhx.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://hyu.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uyn.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lht.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://bli.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://aff.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://pgn.chenzaomai.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://bos.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://emj.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fcy.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://fct.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://twc.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vue.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://miw.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://yak.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://cxo.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zpa.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zdv.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zae.cheryme.top

[E11] 反转字符串
来源：http://xsb.zycfv.cn

Py:   s[::-1]
来源：http://uiq.nwbrower.top

PHP:  strrev($s);
来源：http://gvs.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://gkt.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://fuo.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://eom.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jgv.tian-w.cn

Ruby: s.reverse
来源：http://ldv.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://vgu.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://yjf.yj20258.top

Py:   s.count("a")
来源：http://uep.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://kre.birdmap.top

JS:   s.split("a").length - 1
来源：http://qsi.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://xrj.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uqn.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://dna.chenlongwang.top

Ruby: s.count("a")
来源：http://msh.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://wdp.ydzc1.top

[E13] 逐字符遍历
来源：http://xyd.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://xom.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jcs.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://xds.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vbn.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://umq.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tdv.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yyg.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oog.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://pzp.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lhn.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eel.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ijy.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fqz.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vkt.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zxc.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hrj.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vom.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://ete.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xdd.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://czc.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wpq.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aai.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yjb.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wss.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mbe.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zfs.xinyue.icu

[E16] 数字千分位
来源：http://wrh.wangdashe.top

Py:   f"{1234567:,}"
来源：http://pgx.shuidangran.top

PHP:  number_format(1234567);
来源：http://hbh.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wyd.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gcc.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxy.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vym.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hbq.yongpay.top

C#:   1234567.ToString("N0")
来源：http://kva.cqqwz.cn

[E17] 首字母大写
来源：http://abe.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pxi.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://kul.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://urv.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lbo.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jna.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://erq.0kj1m.cn

Ruby: s.capitalize
来源：http://bgj.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pea.sweek.top

[E18] 模板占位符替换
来源：http://grc.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bmu.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kwr.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uqt.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wsk.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vqx.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ich.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lkf.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dmm.daria6918.cn

[E19] 多行文本按行拆分
来源：http://qja.havefunace.top

Py:   s.splitlines()
来源：http://gvo.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xot.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://omh.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://gjg.yj202588.top

Java: s.lines().toList()
来源：http://eqc.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://ugi.bjfxy.top

Ruby: s.lines
来源：http://phq.tanke756.top

C#:   s.Split('\n')
来源：http://olj.sysykeji.top

[E20] 判断字符串是否为空
来源：http://fws.nwbrower.top

Py:   if not s:
来源：http://zzq.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bpf.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yxc.sxryk.cn

TS:   if (s === "") {}
来源：http://eai.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://wef.zhijiandao.cn

Go:   if s == "" {}
来源：http://pxs.ydzc1.top

Ruby: if s.empty?
来源：http://eoq.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://phf.havefunace.top

[E21] 超长截断加省略号
来源：http://cyg.meibo888.top


<!-- 参考信息 -->