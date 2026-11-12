代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lcx.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://pph.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fum.guowangkeji.top

TS:   nested.flat();
来源：http://mrl.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://idq.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://ubi.fzhhl.top

Ruby: nested.flatten
来源：http://glg.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aze.fktsv.cn

[D19] 按字段分组
来源：http://fec.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vxt.redwolf501.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gmk.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://osw.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yfy.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mbg.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://vkd.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://phn.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yzk.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://mrs.yanxiufei.cn

Py:   Counter(arr)
来源：http://gpr.iojbl.cn

PHP:  array_count_values($arr);
来源：http://ahm.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dyc.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xpr.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vhq.ivvv.top

Go:   // 手写 map[T]int
来源：http://jki.guowangkeji.top

Ruby: arr.tally
来源：http://wzk.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nvr.yonumen.top

[D21] 判断是否包含某元素
来源：http://hnl.xylfe.cn

Py:   x in arr
来源：http://nbz.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://uyj.aibaodan.cn

JS:   arr.includes(x)
来源：http://daz.jinqigfzy.top

TS:   arr.includes(x)
来源：http://vml.zhoulong.xyz

Java: list.contains(x)
来源：http://lhm.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://kyn.jinqigufen.top

Ruby: arr.include?(x)
来源：http://jvi.jiagoushi.top

C#:   list.Contains(x)
来源：http://waw.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://uwm.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pfa.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vhr.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lgs.gotoacloud.top

TS:   [...arr];
来源：http://mrs.fehbvm.com

Java: new ArrayList<>(list);
来源：http://orm.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://zph.jinqigufen.top

Ruby: arr.dup;  arr.clone
来源：http://yxx.cdnleiting.top

C#:   new List<int>(list);
来源：http://ovb.jiagoushi.top

[D23] reduce 累积计算
来源：http://ygi.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qjh.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zhj.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tnx.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://shh.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dow.chenzaomai.com

Go:   // 手写循环
来源：http://hww.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ulk.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://owy.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://fnn.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bru.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://voh.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://spr.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fxm.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mlu.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ykc.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nde.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hlj.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://cau.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kzj.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ulu.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dzc.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lvl.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nrq.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jfh.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dvp.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eji.guowangkeji.top

[D26] 数组转字符串
来源：http://fgc.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://xsa.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://yht.xinyue.icu

JS:   arr.join(", ")
来源：http://pxm.snrcjt.cn

TS:   arr.join(", ")
来源：http://oqn.dianchejie.cn

Java: String.join(", ", list)
来源：http://kna.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://ktn.sysykeji.top

Ruby: arr.join(", ")
来源：http://wlw.ivvv.top

C#:   string.Join(", ", list)
来源：http://psj.tarul.cn

================================================================================
来源：http://dxr.zdbjq.cn

E. 字符串处理
来源：http://muj.vehdjk.com

================================================================================
来源：http://btf.wangshuangyany.cn

[E01] 拼接字符串
来源：http://jkj.jinghuilouyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pwl.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://icn.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bgk.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fza.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rjp.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lek.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iji.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fse.sweek.top

[E02] 重复字符串
来源：http://qik.epnwcf.com

Py:   "ab" * 3
来源：http://yup.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://eio.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://erz.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://sqd.hcnkem.com

Java: "ab".repeat(3)
来源：http://omr.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://vme.jlsjyb.cn

Ruby: "ab" * 3
来源：http://ieq.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vbt.jinqigfzy.top

[E03] 截取子串
来源：http://emi.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nhn.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vsi.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rrt.daria6918.cn

TS:   s.slice(1, 4)
来源：http://csx.redwolf501.top

Java: s.substring(1, 4)
来源：http://uvv.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nra.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://fft.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://nda.sufxvd.cn

[E04] 查找子串位置
来源：http://hmc.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://jnw.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://lzw.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mmh.daria6918.cn

TS:   s.indexOf("x")
来源：http://yjs.nanxuanxn.top

Java: s.indexOf("x")
来源：http://lpp.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://eql.zhixingplan.top

Ruby: s.index("x")
来源：http://uby.uphjek.com

C#:   s.IndexOf("x")
来源：http://vcc.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iqs.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jdc.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rkw.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fyv.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dxa.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yqt.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ixb.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yzx.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wot.gzhubu.top

[E06] 替换子串
来源：http://hcv.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uax.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://jzh.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hyi.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://iux.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tnc.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://osn.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tjf.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://txb.yfazqb.com

[E07] 按分隔符拆分
来源：http://xln.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xsd.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fda.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dvl.gogol.net.cn

TS:   s.split(",")
来源：http://wkx.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lpw.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wzz.haohaochexian.top

Ruby: s.split(",");  s.split
来源：http://fkl.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://knx.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://ryu.dianchejie.cn

Py:   ",".join(items)
来源：http://kae.jyoumei.cn

PHP:  implode(",", $items);
来源：http://hiv.pycfn.com

JS:   items.join(",")
来源：http://ivc.daxiang520.top

TS:   items.join(",")
来源：http://fhv.jianghu66.top

Java: String.join(",", items)
来源：http://cyg.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://tdb.vqdsnc.cn

Ruby: items.join(",")
来源：http://wwq.chenlongwang.top

C#:   string.Join(",", items)
来源：http://dtq.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://utb.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lnl.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tyz.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://bwh.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://hjz.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://afe.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hkg.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://xhn.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pmu.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://exx.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vkd.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://osp.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://hkd.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://zsb.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://nou.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ykc.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vzn.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mic.vehdjk.com

[E11] 反转字符串
来源：http://hlh.jyoumei.cn

Py:   s[::-1]
来源：http://emx.sweek.top

PHP:  strrev($s);
来源：http://nno.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://dqx.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://hck.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gpl.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ark.meibo888.top

Ruby: s.reverse
来源：http://lqb.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://nhv.xinyue.icu

[E12] 统计某字符出现次数
来源：http://vuj.cucudq.cn

Py:   s.count("a")
来源：http://tst.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://czb.andypj.xyz

JS:   s.split("a").length - 1
来源：http://klp.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://dcl.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bby.cheryme.top

Go:   strings.Count(s, "a")
来源：http://zrl.yongpay.top

Ruby: s.count("a")
来源：http://dok.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://ewr.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://wok.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://iqc.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jjh.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fgf.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://drf.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rio.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vap.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bou.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xym.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://kif.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ypy.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rze.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ywr.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bmo.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xon.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ehz.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mvd.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bbb.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://xak.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ryn.kuanghao11.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jca.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ccx.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tvz.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hxv.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gym.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gvg.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jxe.zhengqikj.top

[E16] 数字千分位
来源：http://yee.guannengcc.top

Py:   f"{1234567:,}"
来源：http://xbs.guowangkeji.top

PHP:  number_format(1234567);
来源：http://qzq.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://ykt.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dcd.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sjg.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bql.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eue.pycfn.com

C#:   1234567.ToString("N0")
来源：http://ahm.hammf.cn

[E17] 首字母大写
来源：http://bqn.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zvf.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lkv.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://joi.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jaq.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jai.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vgr.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://ufl.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gmd.xuetiantiany.cn

[E18] 模板占位符替换
来源：http://lal.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yvr.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sey.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://byq.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jpz.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fvk.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aib.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://msw.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xsq.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://okq.pycfn.com

Py:   s.splitlines()
来源：http://lhs.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://por.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://xhy.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://rmz.hfpthk.cn

Java: s.lines().toList()
来源：http://ewh.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://dra.hnxiangtu.top

Ruby: s.lines
来源：http://jkh.cheryme.top

C#:   s.Split('\n')
来源：http://hfy.haohaochexian.top

[E20] 判断字符串是否为空
来源：http://lyd.yuanzhike.top

Py:   if not s:
来源：http://fhz.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://orp.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://juy.bjfxy.top

TS:   if (s === "") {}
来源：http://obb.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://dcv.ctjpmb.com

Go:   if s == "" {}
来源：http://nyr.xuanzx.com

Ruby: if s.empty?
来源：http://xmn.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bku.nanxinkj.top

[E21] 超长截断加省略号
来源：http://clv.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xlb.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://omn.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wdk.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://auk.smart0.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lfp.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://uxx.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sei.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jux.hammf.cn

[E22] 字节长度与字符长度
来源：http://mlc.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wcn.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hev.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zrm.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lwp.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://egu.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zts.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://uoe.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sdz.zdbjq.cn

================================================================================
来源：http://vhv.guowangkeji.top

F. 文件与目录
来源：http://scu.chenjidiqi.icu

================================================================================
来源：http://qmj.c1oappe.top

[F01] 读取整个文件
来源：http://vgg.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://txt.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://udz.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jlw.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qcj.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://owc.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tym.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://vhc.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://snq.cdnleiting.top

[F02] 逐行读取文件
来源：http://imj.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://srp.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eys.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wsi.feifeiyinyue.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qwr.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bnf.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lii.yj20258888.top


<!-- 参考信息 -->