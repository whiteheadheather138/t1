代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cjd.zhengqikj.top

Go:   // 手写双层循环
来源：http://ygy.zhixingplan.top

Ruby: nested.flatten
来源：http://zhb.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ahf.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://muf.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hez.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zwr.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xft.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kof.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kih.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://age.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://dxc.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ngn.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://jsw.pengpengdd.cyou

Py:   Counter(arr)
来源：http://isw.zhijiandao.cn

PHP:  array_count_values($arr);
来源：http://vzt.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rru.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cql.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bfk.tanke756.top

Go:   // 手写 map[T]int
来源：http://wyh.ybcxt.top

Ruby: arr.tally
来源：http://ews.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qsy.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://pcl.dianchejie.cn

Py:   x in arr
来源：http://jqy.mhx1999.top

PHP:  in_array($x, $arr, true);
来源：http://wmp.gzhubu.top

JS:   arr.includes(x)
来源：http://dcu.hysaishi.cn

TS:   arr.includes(x)
来源：http://mfy.feifeiyinyue.top

Java: list.contains(x)
来源：http://fyp.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://sgb.hnqzz.top

Ruby: arr.include?(x)
来源：http://lww.hcnkem.com

C#:   list.Contains(x)
来源：http://vqv.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://nku.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hgq.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zaa.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mck.yj20258888.top

TS:   [...arr];
来源：http://ona.zhengqikj.top

Java: new ArrayList<>(list);
来源：http://fif.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://ret.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://csn.jqgfzy.top

C#:   new List<int>(list);
来源：http://usu.bbcook.cn

[D23] reduce 累积计算
来源：http://fns.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hau.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ozq.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ukn.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqw.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vcd.chenlongwang.top

Go:   // 手写循环
来源：http://rjc.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sco.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xyq.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://yje.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://viu.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fas.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://obn.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cjp.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wwd.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wca.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://voe.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nuk.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://kjv.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://djj.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lbf.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dwz.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uei.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pgf.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://can.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://byc.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://poi.jinqigufen.top

[D26] 数组转字符串
来源：http://aba.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://aab.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://kcr.316326.xyz

JS:   arr.join(", ")
来源：http://jdl.jinqigufen.top

TS:   arr.join(", ")
来源：http://mfb.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://hnx.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://ctu.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://gdm.yonumen.top

C#:   string.Join(", ", list)
来源：http://wfo.vehdjk.com

================================================================================
来源：http://xwp.cqqwz.cn

E. 字符串处理
来源：http://gkl.ctjpmb.com

================================================================================
来源：http://ysh.redwolf501.top

[E01] 拼接字符串
来源：http://ibd.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sbi.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jls.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://evf.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ahi.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ice.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mvn.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://twu.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lzs.nanxinkj.top

[E02] 重复字符串
来源：http://cie.xziqi.cn

Py:   "ab" * 3
来源：http://sfx.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://eiz.daxiang520.top

JS:   "ab".repeat(3)
来源：http://pck.daria6918.cn

TS:   "ab".repeat(3)
来源：http://qwp.meibo888.top

Java: "ab".repeat(3)
来源：http://yor.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://jff.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://hau.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gzs.zhengqikj.top

[E03] 截取子串
来源：http://bqh.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cge.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yfj.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://egz.fzhhl.top

TS:   s.slice(1, 4)
来源：http://etc.hammf.cn

Java: s.substring(1, 4)
来源：http://qib.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rrm.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ert.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://itu.svipenyu.cn

[E04] 查找子串位置
来源：http://kqn.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://jum.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://iqc.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rge.tanke756.top

TS:   s.indexOf("x")
来源：http://lgy.52xcode.cn

Java: s.indexOf("x")
来源：http://tfk.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://hxh.yvedp.cn

Ruby: s.index("x")
来源：http://cih.zhiwuduotai.top

C#:   s.IndexOf("x")
来源：http://cyc.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xek.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kyk.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://byx.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nbl.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://kjv.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ljo.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ehz.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rmv.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fcs.jyoumei.cn

[E06] 替换子串
来源：http://rgw.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rnc.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://dyl.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zsp.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://toy.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hfp.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ake.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dfs.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://ett.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://iva.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ffc.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dua.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://eda.fktsv.cn

TS:   s.split(",")
来源：http://akf.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://shf.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bjc.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://plr.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nia.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://msa.zhengqikj.top

Py:   ",".join(items)
来源：http://bgs.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://rve.jinqigufen.top

JS:   items.join(",")
来源：http://mkw.andypj.xyz

TS:   items.join(",")
来源：http://fhq.mhx1999.top

Java: String.join(",", items)
来源：http://mla.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://wdd.gotoacloud.top

Ruby: items.join(",")
来源：http://lbr.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://edy.redwolf501.top

[E09] 去除所有空白字符
来源：http://bvb.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vzd.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qdw.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://wvp.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://hmr.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://qah.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rpj.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://rmx.wangshuangyany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zmd.zhengqikj.top

[E10] 左侧补零 / 定长填充
来源：http://fvr.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rqj.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://boj.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://eev.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://orm.bjfxy.top

Java: String.format("%03d", 7)
来源：http://zqe.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://khq.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wfi.hnxiangtu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xuj.cucudq.cn

[E11] 反转字符串
来源：http://jos.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://apw.fzhhl.top

PHP:  strrev($s);
来源：http://nal.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://uzg.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://sxw.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bzt.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lct.cdnleiting.top

Ruby: s.reverse
来源：http://vkk.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://ege.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://mqy.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://cok.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://sak.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://tyd.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://xaf.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mtu.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://zzr.sjlbkw.cn

Ruby: s.count("a")
来源：http://nna.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://kgc.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://mwk.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://npx.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yfd.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://big.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://qxn.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://koa.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uto.ivvv.top

Ruby: s.each_char { |ch| puts ch }
来源：http://glz.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dib.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://bku.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xpp.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fvo.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rrl.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://icv.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hua.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gbe.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zbs.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lxh.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://wwq.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://cam.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hkg.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ghs.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ymp.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ifl.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nio.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jct.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bjj.hammf.cn

[E16] 数字千分位
来源：http://rxq.hcnkem.com

Py:   f"{1234567:,}"
来源：http://dyu.epnwcf.com

PHP:  number_format(1234567);
来源：http://wwy.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ryo.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hpx.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uey.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://akd.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fvi.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://vqw.zhoulong.xyz

[E17] 首字母大写
来源：http://zqo.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rkn.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aeo.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfs.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fpr.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rgg.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://plm.zhengqikj.top

Ruby: s.capitalize
来源：http://nux.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://koo.svipenyu.cn

[E18] 模板占位符替换
来源：http://kub.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://twy.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hie.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://jzs.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qyd.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ojr.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nkm.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dth.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ori.fehbvm.com

[E19] 多行文本按行拆分
来源：http://xvq.shangyingyoupin.top

Py:   s.splitlines()
来源：http://bdh.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ohj.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://one.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://eet.tian-w.cn

Java: s.lines().toList()
来源：http://jwc.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://hnj.zhaomingkeji.xyz

Ruby: s.lines
来源：http://gjk.sysykeji.top

C#:   s.Split('\n')
来源：http://gks.yonumen.top

[E20] 判断字符串是否为空
来源：http://snx.hysaishi.cn

Py:   if not s:
来源：http://fri.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://esy.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zbw.cheryme.top

TS:   if (s === "") {}
来源：http://jqv.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://qrt.xuanzx.com

Go:   if s == "" {}
来源：http://qov.yueranfly.top

Ruby: if s.empty?
来源：http://dsc.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nqi.daria6918.cn

[E21] 超长截断加省略号
来源：http://wdu.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bhq.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nny.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lfe.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynd.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hol.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://bim.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://okf.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oux.yfazqb.com

[E22] 字节长度与字符长度
来源：http://tln.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qlm.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtd.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kae.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kgp.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wru.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tyv.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://qtf.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mry.meibo888.top

================================================================================
来源：http://fea.uphjek.com

F. 文件与目录
来源：http://pet.nanxuanxn.top

================================================================================
来源：http://zuv.chenzaomai.com

[F01] 读取整个文件
来源：http://aiy.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ooh.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://qdb.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hmd.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dgf.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ydh.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://acx.meibo888.top

Ruby: File.read("a.txt")
来源：http://dmv.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://caj.yfazqb.com

[F02] 逐行读取文件
来源：http://yga.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yqx.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pkm.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ten.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tsa.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wcx.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqi.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nfi.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sdc.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://wgu.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mkg.cashguo.top


<!-- 参考信息 -->