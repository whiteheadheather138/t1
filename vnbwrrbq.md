代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://egk.yuanzhike.top

Go:   // 手写循环
来源：http://ida.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://alk.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gdn.shuidangran.top

[D15] 去重
来源：http://nnd.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qda.ehwqpu.com

PHP:  array_unique($arr);
来源：http://bts.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://kry.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://dec.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jck.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://bsq.hysaishi.cn

Ruby: arr.uniq
来源：http://ium.yongpay.top

C#:   list.Distinct().ToList()
来源：http://zfx.yuxming.cn

[D16] 求和与平均值
来源：http://wxf.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xjd.chenlongwang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gmd.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cwb.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsf.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wpc.zhijiandao.cn

Go:   // 手写循环累加
来源：http://ogj.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oxo.sweek.top

C#:   list.Sum();  list.Average()
来源：http://her.0kj1m.cn

[D17] 最大值与最小值
来源：http://miw.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://wno.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://hdn.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tvs.redwolf501.top

TS:   Math.max(...arr);
来源：http://hjr.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ipl.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uip.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://avz.yj202588.top

C#:   list.Max();  list.Min()
来源：http://sra.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://jyd.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kwx.jlsjyb.cn

PHP:  array_merge(...$nested);
来源：http://yuy.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://umg.mhx1999.top

TS:   nested.flat();
来源：http://pkr.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rwt.haohaochexian.top

Go:   // 手写双层循环
来源：http://nwk.jqgufenzy.top

Ruby: nested.flatten
来源：http://ved.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eqq.shanyushiyangtech.top

[D19] 按字段分组
来源：http://ksu.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://krq.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wgb.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://htw.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gvd.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xjq.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://rud.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rst.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jpw.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://rcg.yvedp.cn

Py:   Counter(arr)
来源：http://osa.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://ijb.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ctc.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ljh.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dxn.aibaodan.cn

Go:   // 手写 map[T]int
来源：http://rsm.ybcxt.top

Ruby: arr.tally
来源：http://qpm.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kdm.cheryme.top

[D21] 判断是否包含某元素
来源：http://djc.fzhhl.top

Py:   x in arr
来源：http://xmh.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://qdz.xziqi.cn

JS:   arr.includes(x)
来源：http://rxa.nwbrower.top

TS:   arr.includes(x)
来源：http://bsd.chenjidiqi.icu

Java: list.contains(x)
来源：http://djz.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://pyo.mhx1999.top

Ruby: arr.include?(x)
来源：http://cmi.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://olf.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://sbs.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://elq.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fvp.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sgl.sxryk.cn

TS:   [...arr];
来源：http://zwm.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://dgb.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://luu.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://kwd.fengsongda.top

C#:   new List<int>(list);
来源：http://cpi.0kj1m.cn

[D23] reduce 累积计算
来源：http://eml.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pyj.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://piv.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://apd.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mpg.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://huh.svipenyu.cn

Go:   // 手写循环
来源：http://dgv.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qra.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ryh.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://ita.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://olz.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xbk.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fup.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wib.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kex.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wsv.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cxr.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qnx.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://ysm.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fit.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fxd.hfpthk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jje.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sid.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uue.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://edd.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tdf.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xul.daria6918.cn

[D26] 数组转字符串
来源：http://rjv.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://wgo.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://cge.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://vhq.guannengcc.top

TS:   arr.join(", ")
来源：http://ebc.hcnkem.com

Java: String.join(", ", list)
来源：http://vgy.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://qwa.hnqzz.top

Ruby: arr.join(", ")
来源：http://vzy.hnqzz.top

C#:   string.Join(", ", list)
来源：http://lwk.daxiang520.top

================================================================================
来源：http://mnq.zdqjudy.top

E. 字符串处理
来源：http://shc.shangyingyoupin.top

================================================================================
来源：http://axs.xziqi.cn

[E01] 拼接字符串
来源：http://qjd.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jyl.chenjidiqi.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wgj.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ojf.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://chl.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nnf.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sto.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cpl.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xbh.zhongyouzk.top

[E02] 重复字符串
来源：http://tew.xinyue.icu

Py:   "ab" * 3
来源：http://xjw.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://tru.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://yex.cashguo.top

TS:   "ab".repeat(3)
来源：http://ahr.ydzc1.top

Java: "ab".repeat(3)
来源：http://nhr.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://cxo.cdnleiting.top

Ruby: "ab" * 3
来源：http://fek.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hcp.tianlin.xyz

[E03] 截取子串
来源：http://oyz.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yik.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://chn.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvs.nwbrower.top

TS:   s.slice(1, 4)
来源：http://nqf.yangfankeji.com

Java: s.substring(1, 4)
来源：http://hah.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wep.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://sjn.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://ytt.zhengqikj.top

[E04] 查找子串位置
来源：http://ogj.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://erp.tarul.cn

PHP:  strpos($s, "x");
来源：http://aap.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ynh.yuanzhike.top

TS:   s.indexOf("x")
来源：http://tru.tian-w.cn

Java: s.indexOf("x")
来源：http://xev.ehwqpu.com

Go:   strings.Index(s, "x")
来源：http://hqp.fehbvm.com

Ruby: s.index("x")
来源：http://pbn.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://znd.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://idv.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ipj.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ckj.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lwq.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lxi.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://czk.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://suy.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nxi.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nlh.chenlongwang.top

[E06] 替换子串
来源：http://fxo.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qjv.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://zxy.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wri.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://wzd.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iqd.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://epz.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nom.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://bvy.52xcode.cn

[E07] 按分隔符拆分
来源：http://mjq.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nfd.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mlh.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nbk.bbcook.cn

TS:   s.split(",")
来源：http://dxw.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://pza.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ouq.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://ptd.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fqk.tian-w.cn

[E08] 数组按分隔符合并
来源：http://csa.yuxming.cn

Py:   ",".join(items)
来源：http://uqf.yj20258.top

PHP:  implode(",", $items);
来源：http://oad.yj20258888.top

JS:   items.join(",")
来源：http://qiu.pengpengdd.cyou

TS:   items.join(",")
来源：http://wlx.cheryme.top

Java: String.join(",", items)
来源：http://phy.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://ssy.nanxuanxn.top

Ruby: items.join(",")
来源：http://mfs.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://moh.dianchejie.cn

[E09] 去除所有空白字符
来源：http://jtu.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cme.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aai.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://glc.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://epr.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://tca.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rrx.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ksz.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fvy.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://hyq.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lso.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://urq.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://ufl.sweek.top

TS:   "7".padStart(3, "0")
来源：http://soc.ybcxt.top

Java: String.format("%03d", 7)
来源：http://iym.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ycn.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vya.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ksn.mhx1999.top

[E11] 反转字符串
来源：http://txa.haohaochexian.top

Py:   s[::-1]
来源：http://bkb.zhijiandao.cn

PHP:  strrev($s);
来源：http://gcj.tanke756.top

JS:   [...s].reverse().join("")
来源：http://nrk.yonumen.top

TS:   [...s].reverse().join("")
来源：http://nyn.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hth.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ugx.fzhhl.top

Ruby: s.reverse
来源：http://sqw.zhijiandao.cn

C#:   new string(s.Reverse().ToArray())
来源：http://suz.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://mwg.uphjek.com

Py:   s.count("a")
来源：http://tey.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://fma.tanke756.top

JS:   s.split("a").length - 1
来源：http://xld.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://ngv.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://whs.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://wna.c1oappe.top

Ruby: s.count("a")
来源：http://amb.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://fkq.sxryk.cn

[E13] 逐字符遍历
来源：http://rly.ydzc1.top

Py:   for ch in s: print(ch)
来源：http://phv.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vld.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hko.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hpf.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nmd.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kiy.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tlz.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vwm.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://alq.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ebl.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://uhf.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ltk.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iii.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tnt.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mtx.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://esy.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jku.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://yox.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pmy.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tgf.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://par.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://gfr.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hlt.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yrq.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://myz.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lpc.shanyushiyangkeji.top

[E16] 数字千分位
来源：http://awv.hnqzz.top

Py:   f"{1234567:,}"
来源：http://nzi.jyoumei.cn

PHP:  number_format(1234567);
来源：http://lqe.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://noh.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kad.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vai.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ddt.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://drp.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://pwg.cucudq.cn

[E17] 首字母大写
来源：http://gvd.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wvn.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nbd.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xid.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zuc.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lzb.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hyi.fengsongda.top

Ruby: s.capitalize
来源：http://jws.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fac.cqqwz.cn

[E18] 模板占位符替换
来源：http://wjb.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nrv.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fqg.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fww.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cxm.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wnh.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dzd.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uuf.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ksg.shuidangran.top

[E19] 多行文本按行拆分
来源：http://khy.svipenyu.cn

Py:   s.splitlines()
来源：http://ksd.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gst.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://zqy.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://ncc.sjlbkw.cn

Java: s.lines().toList()
来源：http://dgo.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://fkv.shanyushiyangtech.top

Ruby: s.lines
来源：http://zhm.cashguo.top

C#:   s.Split('\n')
来源：http://scf.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://sof.fzhhl.top

Py:   if not s:
来源：http://pte.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kkv.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pcv.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://fbt.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://pyu.zycfv.cn

Go:   if s == "" {}
来源：http://dpj.xziqi.cn

Ruby: if s.empty?
来源：http://ihd.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ipb.ydzc1.top

[E21] 超长截断加省略号
来源：http://hvh.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cnq.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lcm.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mrd.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://btl.jinqigfzy.top


<!-- 参考信息 -->