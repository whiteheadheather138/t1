代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qzs.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://ffz.yj20258888.top

[D17] 最大值与最小值
来源：http://nkd.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://iiv.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://pjc.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ymt.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://guo.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://udw.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://abm.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://hkd.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://zbe.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://ccz.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dxu.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://vmi.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ovi.yj202588.top

TS:   nested.flat();
来源：http://dyx.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xqd.haohaochexian.top

Go:   // 手写双层循环
来源：http://eqe.daxiang520.top

Ruby: nested.flatten
来源：http://nen.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cuz.fktsv.cn

[D19] 按字段分组
来源：http://kza.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://urf.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nzh.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cbf.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://iat.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tfa.uphjek.com

Go:   // 手写 map[string][]T
来源：http://hfp.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://itg.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oef.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://anm.zhiwuduotai.top

Py:   Counter(arr)
来源：http://tvb.sysykeji.top

PHP:  array_count_values($arr);
来源：http://wcs.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qwa.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggf.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xfa.hcnkem.com

Go:   // 手写 map[T]int
来源：http://dmw.nanxuanxn.top

Ruby: arr.tally
来源：http://rzr.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lhd.bbcook.cn

[D21] 判断是否包含某元素
来源：http://lfm.zhoulong.xyz

Py:   x in arr
来源：http://zqq.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://oaf.yongpay.top

JS:   arr.includes(x)
来源：http://gef.jqgufenzy.top

TS:   arr.includes(x)
来源：http://byy.meibo888.top

Java: list.contains(x)
来源：http://dnm.nanxuanxn.top

Go:   slices.Contains(arr, x)
来源：http://nev.yj20258.top

Ruby: arr.include?(x)
来源：http://irs.zhongyouzk.top

C#:   list.Contains(x)
来源：http://yia.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://qtv.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://etb.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ajo.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kxa.nwbrower.top

TS:   [...arr];
来源：http://jaa.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://dft.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hpj.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://qbr.fktsv.cn

C#:   new List<int>(list);
来源：http://rlh.yj202588.top

[D23] reduce 累积计算
来源：http://qti.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cww.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qwg.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oyv.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oxl.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eme.ivvv.top

Go:   // 手写循环
来源：http://uxe.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ncq.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tcv.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://ikh.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ozn.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://une.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hce.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yii.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lyd.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lig.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vwu.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xjo.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://zri.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://abi.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gdr.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nzz.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://roh.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://awn.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gfr.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mmv.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sgo.sweek.top

[D26] 数组转字符串
来源：http://zyo.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://bsd.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://fyv.zhaomingkeji.xyz

JS:   arr.join(", ")
来源：http://uhz.xuanzx.com

TS:   arr.join(", ")
来源：http://txq.uphjek.com

Java: String.join(", ", list)
来源：http://fdb.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://oop.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://jpd.hesvh.cn

C#:   string.Join(", ", list)
来源：http://rhi.cucudq.cn

================================================================================
来源：http://shl.zhaomingkeji.xyz

E. 字符串处理
来源：http://ktq.fzhhl.top

================================================================================
来源：http://ggy.yj20258888.top

[E01] 拼接字符串
来源：http://gzm.jinghuilouyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ykm.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xsy.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ycg.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tns.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wck.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vkl.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zvb.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nrm.sjlbkw.cn

[E02] 重复字符串
来源：http://mwp.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://wfc.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://lxe.tarul.cn

JS:   "ab".repeat(3)
来源：http://nis.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://ehx.zdqjudy.top

Java: "ab".repeat(3)
来源：http://ckx.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://xyz.haohaochexian.top

Ruby: "ab" * 3
来源：http://ccw.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xlr.zhongyouzk.top

[E03] 截取子串
来源：http://ifs.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sov.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nrr.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ozj.epnwcf.com

TS:   s.slice(1, 4)
来源：http://xbx.guannengcc.top

Java: s.substring(1, 4)
来源：http://ouf.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eji.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://lku.yongpay.top

C#:   s.Substring(1, 3)
来源：http://lhe.cucudq.cn

[E04] 查找子串位置
来源：http://ilg.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://tcj.ivvv.top

PHP:  strpos($s, "x");
来源：http://xdi.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aon.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://uda.gzhubu.top

Java: s.indexOf("x")
来源：http://qnp.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://dvu.cucudq.cn

Ruby: s.index("x")
来源：http://cra.yueranfly.top

C#:   s.IndexOf("x")
来源：http://rmw.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fcy.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dgs.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fgo.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sek.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ipg.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fnc.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ahz.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qml.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zof.guannengcc.top

[E06] 替换子串
来源：http://kch.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tkk.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://uzy.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tkz.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://cjl.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mbg.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fot.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hoe.havefunace.top

C#:   s.Replace("a", "b")
来源：http://vje.yuanzhike.top

[E07] 按分隔符拆分
来源：http://nqa.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gxu.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dqh.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://npk.cashguo.top

TS:   s.split(",")
来源：http://nyg.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ftd.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zcz.tarul.cn

Ruby: s.split(",");  s.split
来源：http://kdx.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vzo.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://ypc.zhiwuduotai.top

Py:   ",".join(items)
来源：http://auw.ivvv.top

PHP:  implode(",", $items);
来源：http://nvv.iojbl.cn

JS:   items.join(",")
来源：http://fth.zhijiandao.cn

TS:   items.join(",")
来源：http://skd.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://sav.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://hpr.fzhhl.top

Ruby: items.join(",")
来源：http://viu.zhaomingkeji.xyz

C#:   string.Join(",", items)
来源：http://nrm.yj20258888.top

[E09] 去除所有空白字符
来源：http://qmp.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vie.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yxu.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://yar.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://uxk.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://pum.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://pwf.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://hff.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xrh.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://xoh.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://svs.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mjx.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://egm.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://izn.daria6918.cn

Java: String.format("%03d", 7)
来源：http://hrw.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kgl.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jvl.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vfr.redwolf501.top

[E11] 反转字符串
来源：http://vyd.cqqwz.cn

Py:   s[::-1]
来源：http://kki.jinghuilouyu.cn

PHP:  strrev($s);
来源：http://khu.yongpay.top

JS:   [...s].reverse().join("")
来源：http://zrj.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://ylm.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://jta.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jka.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://ucd.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rci.yuxming.cn

[E12] 统计某字符出现次数
来源：http://jhe.sweek.top

Py:   s.count("a")
来源：http://qwq.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://mnh.xuanzx.com

JS:   s.split("a").length - 1
来源：http://xub.aizwys.cn

TS:   s.split("a").length - 1
来源：http://myz.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pmj.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://vqd.316326.xyz

Ruby: s.count("a")
来源：http://nhj.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://fnj.haohaochexian.top

[E13] 逐字符遍历
来源：http://ajv.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://jmf.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bqy.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ahl.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://puw.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pgl.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://auy.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://crv.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iyj.ydzc1.top

[E14] URL 编码与 Base64
来源：http://dzb.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xiw.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fyr.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tjf.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sjo.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://knf.yvedp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jxi.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jsh.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fpx.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://imm.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://meb.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bwa.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://okj.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://uwx.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mvx.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ewr.hongshengwenyu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://boc.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://veu.cdnleiting.top

[E16] 数字千分位
来源：http://uhp.xziqi.cn

Py:   f"{1234567:,}"
来源：http://ocv.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://upp.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://mit.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wnj.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://frk.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qna.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pvo.cqqwz.cn

C#:   1234567.ToString("N0")
来源：http://vna.9152youxi.cn

[E17] 首字母大写
来源：http://gue.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dfw.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fzw.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rxf.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iac.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qft.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xsw.tian-w.cn

Ruby: s.capitalize
来源：http://lub.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xfq.vehdjk.com

[E18] 模板占位符替换
来源：http://dbh.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tsv.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gyr.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ifd.jinqigufen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qkx.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ecu.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dub.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mrc.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pgn.guannengcc.top

[E19] 多行文本按行拆分
来源：http://jzn.iojbl.cn

Py:   s.splitlines()
来源：http://axu.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qwj.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://jmt.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://cwl.wangshuangyany.cn

Java: s.lines().toList()
来源：http://zds.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://pid.daxiang520.top

Ruby: s.lines
来源：http://yno.ehwqpu.com

C#:   s.Split('\n')
来源：http://xts.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://qcd.zhaomingkeji.xyz

Py:   if not s:
来源：http://fwf.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eno.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lnd.xinyue.icu

TS:   if (s === "") {}
来源：http://kfd.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://wya.shuidangran.top

Go:   if s == "" {}
来源：http://vwb.cqqwz.cn

Ruby: if s.empty?
来源：http://ikn.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iop.ybcxt.top

[E21] 超长截断加省略号
来源：http://gvo.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jkk.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://upx.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hic.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gsf.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wxg.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://nsv.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cke.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uay.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://thb.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tvn.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vct.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dpf.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aap.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oat.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://enf.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://kau.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hta.jinghuilouyu.cn

================================================================================
来源：http://agl.yfazqb.com

F. 文件与目录
来源：http://bvb.bbcook.cn

================================================================================
来源：http://nmt.yonumen.top

[F01] 读取整个文件
来源：http://xtj.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ood.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://hbh.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eti.ydzc1.top


<!-- 参考信息 -->