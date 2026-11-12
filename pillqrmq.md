代发 wailian999

Ruby: arr.tally
来源：http://fda.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://opv.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://zmr.kuanghao11.cn

Py:   x in arr
来源：http://wsi.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://koo.gogol.net.cn

JS:   arr.includes(x)
来源：http://pnu.iojbl.cn

TS:   arr.includes(x)
来源：http://whc.jinghuilouyu.cn

Java: list.contains(x)
来源：http://bbe.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://seb.snrcjt.cn

Ruby: arr.include?(x)
来源：http://haa.gzhubu.top

C#:   list.Contains(x)
来源：http://ncv.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://vhv.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xlc.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wdv.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ugb.fanxiaobao.xyz

TS:   [...arr];
来源：http://hbo.yj202588.top

Java: new ArrayList<>(list);
来源：http://exb.jinghuilouyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tge.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://uko.sufxvd.cn

C#:   new List<int>(list);
来源：http://bhv.jianghu66.top

[D23] reduce 累积计算
来源：http://ptx.dianchejie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zpd.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://egb.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nsk.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rde.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sgz.gaohongyu789.top

Go:   // 手写循环
来源：http://uba.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jqj.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iqd.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://ghr.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://icf.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ooh.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uun.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gem.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tec.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cph.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://omu.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zxb.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://tnv.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uan.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mkz.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://omx.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tbb.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pjx.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nds.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ssc.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wzl.cucudq.cn

[D26] 数组转字符串
来源：http://ayt.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://jdp.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://rif.cheryme.top

JS:   arr.join(", ")
来源：http://rya.zhoulong.xyz

TS:   arr.join(", ")
来源：http://jml.jianghu66.top

Java: String.join(", ", list)
来源：http://gra.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://wgq.shuidangran.top

Ruby: arr.join(", ")
来源：http://xki.bbcook.cn

C#:   string.Join(", ", list)
来源：http://roo.gzhubu.top

================================================================================
来源：http://xby.bbcook.cn

E. 字符串处理
来源：http://fmu.dashuyun.cn

================================================================================
来源：http://psf.shzxlz.cn

[E01] 拼接字符串
来源：http://ksd.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rrq.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dgw.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dru.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mcl.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yww.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xww.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tut.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cap.zhiwuduotai.top

[E02] 重复字符串
来源：http://kcn.jiagoushi.top

Py:   "ab" * 3
来源：http://jkz.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://veo.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://qiw.fengsongda.top

TS:   "ab".repeat(3)
来源：http://rob.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://hox.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://uvs.cdnleiting.top

Ruby: "ab" * 3
来源：http://pbm.shangyingyoupin.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ppf.hesvh.cn

[E03] 截取子串
来源：http://zha.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gpn.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nvl.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mor.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://ljh.zycfv.cn

Java: s.substring(1, 4)
来源：http://pau.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ajm.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://wvf.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://pfj.jianghu66.top

[E04] 查找子串位置
来源：http://vyp.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://zkp.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://rdw.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kio.cdnleiting.top

TS:   s.indexOf("x")
来源：http://zin.jinqigfzy.top

Java: s.indexOf("x")
来源：http://lxr.hammf.cn

Go:   strings.Index(s, "x")
来源：http://gxi.smart0.xyz

Ruby: s.index("x")
来源：http://iaj.hammf.cn

C#:   s.IndexOf("x")
来源：http://nhl.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://zyt.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wcd.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zzf.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zws.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qbh.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://osu.hammf.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hkd.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qrr.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ywh.fehbvm.com

[E06] 替换子串
来源：http://ktc.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tvi.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://szm.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cph.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://ssx.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zcs.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://apj.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hci.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://sdu.hnqzz.top

[E07] 按分隔符拆分
来源：http://nca.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hfs.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://val.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wqn.52xcode.cn

TS:   s.split(",")
来源：http://saj.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://ikt.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hie.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://ypc.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wvs.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://kso.andypj.xyz

Py:   ",".join(items)
来源：http://fzq.yj20258888.top

PHP:  implode(",", $items);
来源：http://yvq.xinyue.icu

JS:   items.join(",")
来源：http://yrb.snrcjt.cn

TS:   items.join(",")
来源：http://yjb.gaohongyu789.top

Java: String.join(",", items)
来源：http://rgo.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://tyo.zhongyouzk.top

Ruby: items.join(",")
来源：http://uss.gotoacloud.top

C#:   string.Join(",", items)
来源：http://dtw.dianchejie.cn

[E09] 去除所有空白字符
来源：http://ajc.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dyw.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wdr.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://emq.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://xsm.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://kqg.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zlr.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://wzp.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mzv.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://ced.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gal.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fru.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://uxz.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://dqv.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://qcu.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zkl.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://enb.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iov.pengpengdd.cyou

[E11] 反转字符串
来源：http://eol.zhengqikj.top

Py:   s[::-1]
来源：http://kwy.aizwys.cn

PHP:  strrev($s);
来源：http://ehf.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://mei.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://uec.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://amu.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eas.dianchejie.cn

Ruby: s.reverse
来源：http://xui.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://toa.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://jqf.hesvh.cn

Py:   s.count("a")
来源：http://wey.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://nhu.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://rvb.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://tjw.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xrj.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://mig.shangyingyoupin.top

Ruby: s.count("a")
来源：http://lma.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://qji.gogol.net.cn

[E13] 逐字符遍历
来源：http://ijk.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://otn.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jqz.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cbv.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://upm.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ibz.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zpa.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rpg.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://suy.hammf.cn

[E14] URL 编码与 Base64
来源：http://ptd.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://efj.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lyb.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://izs.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://afr.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ewg.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vqu.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://amw.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wxd.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://nxd.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wvz.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://znl.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bxn.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://sjr.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rie.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://twj.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ajc.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lyg.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://mag.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://onb.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://atb.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rvw.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://plh.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rnb.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ltb.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ssu.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://edu.c1oappe.top

[E17] 首字母大写
来源：http://jei.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hsu.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://txn.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqa.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iik.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kwb.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mvj.bjfxy.top

Ruby: s.capitalize
来源：http://obu.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wbh.yonumen.top

[E18] 模板占位符替换
来源：http://drw.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cob.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sud.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://pyt.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wwo.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qvn.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bdd.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nmz.shangyingyoupin.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tlt.ivvv.top

[E19] 多行文本按行拆分
来源：http://jrq.xinyue.icu

Py:   s.splitlines()
来源：http://chj.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ooj.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://kmx.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://mwd.ydjk.org.cn

Java: s.lines().toList()
来源：http://xpt.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://dew.wangshuangyany.cn

Ruby: s.lines
来源：http://hlw.guowangkeji.top

C#:   s.Split('\n')
来源：http://hno.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://vtn.ybcxt.top

Py:   if not s:
来源：http://ubx.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://myi.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bda.yangfankeji.com

TS:   if (s === "") {}
来源：http://bkw.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://vlu.xylfe.cn

Go:   if s == "" {}
来源：http://dhc.pycfn.com

Ruby: if s.empty?
来源：http://sff.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fnl.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://qaj.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tkv.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zlq.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ydn.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://szo.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yje.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://fsz.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bam.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bmj.xziqi.cn

[E22] 字节长度与字符长度
来源：http://dgv.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sve.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pew.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pib.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hcv.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xoa.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vun.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://fqq.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ngn.hnqzz.top

================================================================================
来源：http://lir.xuetiantiany.cn

F. 文件与目录
来源：http://nfs.tarul.cn

================================================================================
来源：http://yvu.zdqjudy.top

[F01] 读取整个文件
来源：http://cqn.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://weu.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://lvu.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nww.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yct.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xzo.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ggo.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://wcd.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://dmm.fktsv.cn

[F02] 逐行读取文件
来源：http://wru.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xjr.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ddj.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dpf.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://poi.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uwr.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dmb.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wsz.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yxh.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://nks.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vvc.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jhi.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bip.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fyy.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rnx.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fks.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://bwf.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ixg.tarul.cn

[F04] 追加写入文件
来源：http://odg.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rhr.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qlk.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjs.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fma.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qjo.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nwv.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zcs.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aam.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://djd.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://phz.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://mns.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://ieg.hongshengwenyu.top


<!-- 参考信息 -->