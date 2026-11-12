代发 wailian999

[D15] 去重
来源：http://ipv.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://exg.nanxinkj.top

PHP:  array_unique($arr);
来源：http://dah.gzhubu.top

JS:   [...new Set(arr)]
来源：http://dcs.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://cxm.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bul.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://ouq.ppjwa.cn

Ruby: arr.uniq
来源：http://dnk.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://iwf.epnwcf.com

[D16] 求和与平均值
来源：http://asi.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yxd.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wcj.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jvc.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zqc.xylfe.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bna.fktsv.cn

Go:   // 手写循环累加
来源：http://qlf.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cax.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://fbn.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://qey.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://vht.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://fup.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hde.jqgfzy.top

TS:   Math.max(...arr);
来源：http://lwt.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rnl.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vzi.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://nrl.yongpay.top

C#:   list.Max();  list.Min()
来源：http://ebg.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://egy.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bsj.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://xpl.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iee.fktsv.cn

TS:   nested.flat();
来源：http://iqi.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jbu.xylfe.cn

Go:   // 手写双层循环
来源：http://gza.fehbvm.com

Ruby: nested.flatten
来源：http://oka.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vqo.gotoacloud.top

[D19] 按字段分组
来源：http://pfa.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tlu.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vjn.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bnz.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jnv.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ppm.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://hfg.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hci.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ttz.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://hsm.zdqjudy.top

Py:   Counter(arr)
来源：http://jrx.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://kqo.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kau.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eft.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hem.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://zpm.havefunace.top

Ruby: arr.tally
来源：http://ckv.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ydr.sysykeji.top

[D21] 判断是否包含某元素
来源：http://ypo.0kj1m.cn

Py:   x in arr
来源：http://tdw.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://kcs.pycfn.com

JS:   arr.includes(x)
来源：http://zuq.fehbvm.com

TS:   arr.includes(x)
来源：http://jnn.tianlin.xyz

Java: list.contains(x)
来源：http://jpw.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://emu.gotoacloud.top

Ruby: arr.include?(x)
来源：http://pui.fengsongda.top

C#:   list.Contains(x)
来源：http://dhj.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://zcq.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ttk.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kqv.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yjk.zhengqikj.top

TS:   [...arr];
来源：http://vds.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://ybd.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://gqr.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://enr.c1oappe.top

C#:   new List<int>(list);
来源：http://ybt.xziqi.cn

[D23] reduce 累积计算
来源：http://mzl.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mew.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://new.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zkr.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://scv.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ydm.ivvv.top

Go:   // 手写循环
来源：http://owg.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eyg.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yyz.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://ksf.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mhs.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jmg.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gih.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dib.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ekq.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://omt.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://omn.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jfp.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://fdo.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bwt.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lmk.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ltc.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://frq.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ruj.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qya.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kqx.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ngb.shangyingyoupin.top

[D26] 数组转字符串
来源：http://qev.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://usx.birdmap.top

PHP:  implode(", ", $arr);
来源：http://fru.zdqjudy.top

JS:   arr.join(", ")
来源：http://utv.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://rcw.zhongyouzk.top

Java: String.join(", ", list)
来源：http://bip.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://nwm.pycfn.com

Ruby: arr.join(", ")
来源：http://koj.yueranfly.top

C#:   string.Join(", ", list)
来源：http://cxv.zhongyouzk.top

================================================================================
来源：http://qve.9152youxi.cn

E. 字符串处理
来源：http://jyj.ydzc1.top

================================================================================
来源：http://vqg.aibaodan.cn

[E01] 拼接字符串
来源：http://wtw.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zeb.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mfs.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmo.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mar.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rxp.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ucu.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jhf.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xal.zycfv.cn

[E02] 重复字符串
来源：http://knn.zhijiandao.cn

Py:   "ab" * 3
来源：http://khm.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://nyr.xuanzx.com

JS:   "ab".repeat(3)
来源：http://agb.ybcxt.top

TS:   "ab".repeat(3)
来源：http://mex.gotoacloud.top

Java: "ab".repeat(3)
来源：http://xqb.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://npk.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://fpa.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dym.shanyushiyangkeji.top

[E03] 截取子串
来源：http://ocb.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jxt.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://box.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://edr.bjfxy.top

TS:   s.slice(1, 4)
来源：http://ipy.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://yxg.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nwh.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://ttm.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://zvz.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://vho.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://skj.cucudq.cn

PHP:  strpos($s, "x");
来源：http://feh.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://opg.chenlongwang.top

TS:   s.indexOf("x")
来源：http://ahc.cheryme.top

Java: s.indexOf("x")
来源：http://vcz.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://buu.nanxinkj.top

Ruby: s.index("x")
来源：http://hwz.fehbvm.com

C#:   s.IndexOf("x")
来源：http://lis.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ygb.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://shw.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xfd.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nen.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://evg.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rse.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://apo.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hsx.yj20258888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rlx.cucudq.cn

[E06] 替换子串
来源：http://zuw.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uzk.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://zbl.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ijq.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://oxy.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nnq.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jks.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rys.hammf.cn

C#:   s.Replace("a", "b")
来源：http://ann.uphjek.com

[E07] 按分隔符拆分
来源：http://ujl.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ooj.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hza.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iic.havefunace.top

TS:   s.split(",")
来源：http://thx.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ozc.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yyk.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://vfy.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pmb.bjfxy.top

[E08] 数组按分隔符合并
来源：http://ctd.zhixingplan.top

Py:   ",".join(items)
来源：http://eyu.sysykeji.top

PHP:  implode(",", $items);
来源：http://yez.uphjek.com

JS:   items.join(",")
来源：http://txj.pengpengdd.cyou

TS:   items.join(",")
来源：http://coc.fzhhl.top

Java: String.join(",", items)
来源：http://pny.ivvv.top

Go:   strings.Join(items, ",")
来源：http://tzu.gotoacloud.top

Ruby: items.join(",")
来源：http://cwq.iojbl.cn

C#:   string.Join(",", items)
来源：http://zjj.zycfv.cn

[E09] 去除所有空白字符
来源：http://oal.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vuz.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tsn.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://uxs.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://dei.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://dil.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://rnp.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bzw.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ulo.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://evn.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hvu.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qnc.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://tzn.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://ulv.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://khh.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://jqa.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lwp.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vfq.zhijiandao.cn

[E11] 反转字符串
来源：http://nkt.havefunace.top

Py:   s[::-1]
来源：http://ovd.tarul.cn

PHP:  strrev($s);
来源：http://doo.yj202588.top

JS:   [...s].reverse().join("")
来源：http://ejn.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://ozb.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lle.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://whq.hywenlv.cn

Ruby: s.reverse
来源：http://iwz.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://yrq.yvedp.cn

[E12] 统计某字符出现次数
来源：http://hiw.nanxinkj.top

Py:   s.count("a")
来源：http://kcp.wangdashe.top

PHP:  substr_count($s, "a");
来源：http://msn.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://rhe.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://qop.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qdn.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://fvu.zhiwuduotai.top

Ruby: s.count("a")
来源：http://smy.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://ybv.jlsjyb.cn

[E13] 逐字符遍历
来源：http://hcr.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://voe.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ptc.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zws.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uxi.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qui.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fjb.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://opk.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pqu.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://lyj.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ezt.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mhr.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qyi.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://req.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tfu.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vxz.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dat.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iqq.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://syx.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eon.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oft.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nsr.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://etb.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://inq.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gao.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ofv.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qcl.cqqwz.cn

[E16] 数字千分位
来源：http://gjg.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://laz.cdnleiting.top

PHP:  number_format(1234567);
来源：http://keh.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://jqs.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://yoc.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bkj.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tsw.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ynq.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://ndc.quarkkingdee.top

[E17] 首字母大写
来源：http://wni.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ohl.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mip.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mxu.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sec.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nwc.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jsq.yonumen.top

Ruby: s.capitalize
来源：http://tht.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fsj.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://tjw.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kcm.redwolf501.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lma.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://haw.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mcn.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ymv.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xxa.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://djg.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zcl.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://zqe.shangyingyoupin.top

Py:   s.splitlines()
来源：http://olu.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xqt.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://kzz.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://qnr.sjlbkw.cn

Java: s.lines().toList()
来源：http://sjf.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://isz.smart0.xyz

Ruby: s.lines
来源：http://uji.tarul.cn

C#:   s.Split('\n')
来源：http://zid.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://sbx.dianchejie.cn

Py:   if not s:
来源：http://nnj.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bwm.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jmn.ehwqpu.com

TS:   if (s === "") {}
来源：http://kpg.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://gkm.mhx1999.top

Go:   if s == "" {}
来源：http://pik.quarkkingdee.top

Ruby: if s.empty?
来源：http://ytk.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yle.cucudq.cn

[E21] 超长截断加省略号
来源：http://rqv.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ckj.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tbj.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ykr.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fpg.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vpe.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://ued.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rhf.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zbo.bbcook.cn


<!-- 参考信息 -->