代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://wbd.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://jtp.ivvv.top

TS:   arr.includes(x)
来源：http://viw.pengpengdd.cyou

Java: list.contains(x)
来源：http://gey.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://wtt.pycfn.com

Ruby: arr.include?(x)
来源：http://tsk.yongpay.top

C#:   list.Contains(x)
来源：http://duv.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://kyl.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nwx.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rhm.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tfp.yj202588.top

TS:   [...arr];
来源：http://xdt.xziqi.cn

Java: new ArrayList<>(list);
来源：http://nfu.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://drn.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://dle.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://vtj.zhijiandao.cn

[D23] reduce 累积计算
来源：http://gro.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xcq.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ylp.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wnb.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kqk.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fdd.sysykeji.top

Go:   // 手写循环
来源：http://vmw.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rjt.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bzh.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://nbq.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qdu.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eth.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aee.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bzn.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nbj.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://umf.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gtq.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://abn.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://ycg.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://udq.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gwc.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pgg.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kks.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zdp.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://esa.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pmp.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ioq.hnxiangtu.top

[D26] 数组转字符串
来源：http://jot.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://zhs.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://gya.chenlongwang.top

JS:   arr.join(", ")
来源：http://gwe.chenzaomai.com

TS:   arr.join(", ")
来源：http://wuc.cheryme.top

Java: String.join(", ", list)
来源：http://okj.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://pwh.fengsongda.top

Ruby: arr.join(", ")
来源：http://let.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://xac.c1oappe.top

================================================================================
来源：http://hmj.hysaishi.cn

E. 字符串处理
来源：http://ofz.jiagoushi.top

================================================================================
来源：http://wzf.quarkkingdee.top

[E01] 拼接字符串
来源：http://jgh.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://beg.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jtc.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://all.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hml.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cir.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ern.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nqv.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aud.gogol.net.cn

[E02] 重复字符串
来源：http://rex.sufxvd.cn

Py:   "ab" * 3
来源：http://llb.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://ray.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://jrp.bjfxy.top

TS:   "ab".repeat(3)
来源：http://csk.yuxming.cn

Java: "ab".repeat(3)
来源：http://hod.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://kss.gogol.net.cn

Ruby: "ab" * 3
来源：http://vlp.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ayp.birdmap.top

[E03] 截取子串
来源：http://dlu.chenjidiqi.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qne.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://csq.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kho.sxryk.cn

TS:   s.slice(1, 4)
来源：http://duz.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://kph.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qxa.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://iup.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://fqf.yuxming.cn

[E04] 查找子串位置
来源：http://wdq.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://obo.redwolf501.top

PHP:  strpos($s, "x");
来源：http://dpr.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aos.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://tks.tian-w.cn

Java: s.indexOf("x")
来源：http://ttm.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://gid.cqqwz.cn

Ruby: s.index("x")
来源：http://liv.yvedp.cn

C#:   s.IndexOf("x")
来源：http://ocb.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hyh.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lpt.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ebl.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://brz.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bmk.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://axg.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://add.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hes.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xdh.tanke756.top

[E06] 替换子串
来源：http://gnu.xinyue.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tgn.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://hlg.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://abv.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://vmg.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qor.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ftw.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ofs.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://hed.xziqi.cn

[E07] 按分隔符拆分
来源：http://val.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wju.hywenlv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oep.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sjf.fehbvm.com

TS:   s.split(",")
来源：http://dhb.gzhubu.top

Java: s.split(",");  s.split("\\s+")
来源：http://gzt.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ygu.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://nwq.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://amn.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://zwz.gzhubu.top

Py:   ",".join(items)
来源：http://nma.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://iyg.andypj.xyz

JS:   items.join(",")
来源：http://jrh.dianchejie.cn

TS:   items.join(",")
来源：http://fkd.meibo888.top

Java: String.join(",", items)
来源：http://kya.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://vra.sweek.top

Ruby: items.join(",")
来源：http://vux.dianchejie.cn

C#:   string.Join(",", items)
来源：http://uyn.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://izn.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fci.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bpz.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://yce.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://nmw.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://cue.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://jjv.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://bkw.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vbw.andypj.xyz

[E10] 左侧补零 / 定长填充
来源：http://zqm.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qap.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wmz.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://hqi.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://nbq.xziqi.cn

Java: String.format("%03d", 7)
来源：http://cxx.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uom.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qee.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aoq.snrcjt.cn

[E11] 反转字符串
来源：http://iix.pycfn.com

Py:   s[::-1]
来源：http://wkx.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://qxz.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://ofv.yj20258.top

TS:   [...s].reverse().join("")
来源：http://thc.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ilj.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://drw.hongshengwenyu.top

Ruby: s.reverse
来源：http://bng.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jsu.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://xdz.cdnleiting.top

Py:   s.count("a")
来源：http://ttp.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://ilp.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://dnu.yfazqb.com

TS:   s.split("a").length - 1
来源：http://bgv.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dsa.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://dig.haohaochexian.top

Ruby: s.count("a")
来源：http://gqg.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://jvu.xuanzx.com

[E13] 逐字符遍历
来源：http://atk.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://trl.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vxg.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://axp.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://dxr.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uez.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xld.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lpe.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://igc.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://ixp.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pwm.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://inn.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ojd.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xxd.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tjh.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xcd.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gsn.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://exh.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://oka.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tie.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uur.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://krp.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://efr.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://deg.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lmc.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nln.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lnt.ehwqpu.com

[E16] 数字千分位
来源：http://bdd.shuidangran.top

Py:   f"{1234567:,}"
来源：http://gvj.svipenyu.cn

PHP:  number_format(1234567);
来源：http://ehs.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vey.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://yjw.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rhs.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zbh.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xnn.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://von.ctjpmb.com

[E17] 首字母大写
来源：http://qxz.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://svg.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wtn.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uqm.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nin.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://toe.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tdd.daxiang520.top

Ruby: s.capitalize
来源：http://ays.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nzb.fengsongda.top

[E18] 模板占位符替换
来源：http://agx.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blx.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cxg.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pyn.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bfb.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dud.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vnd.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tfv.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xqk.sweek.top

[E19] 多行文本按行拆分
来源：http://ckq.316326.xyz

Py:   s.splitlines()
来源：http://plb.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xvn.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://gxb.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://mua.havefunace.top

Java: s.lines().toList()
来源：http://vdg.hywenlv.cn

Go:   strings.Split(s, "\n")
来源：http://twn.nwbrower.top

Ruby: s.lines
来源：http://heg.aizwys.cn

C#:   s.Split('\n')
来源：http://jnp.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://ary.ywan-chungtsiang.top

Py:   if not s:
来源：http://zez.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jwh.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rhx.cashguo.top

TS:   if (s === "") {}
来源：http://esb.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://kqt.zhongyouzk.top

Go:   if s == "" {}
来源：http://fac.sysykeji.top

Ruby: if s.empty?
来源：http://aih.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://scq.dianchejie.cn

[E21] 超长截断加省略号
来源：http://kwf.hnxiangtu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://szd.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cpi.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hlk.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lrt.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wvb.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://gmu.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lps.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ris.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://vvi.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gbm.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oyt.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://air.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://clo.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://whq.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qhb.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://vsm.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://waj.wangdashe.top

================================================================================
来源：http://ttz.wangdashe.top

F. 文件与目录
来源：http://dly.meibo888.top

================================================================================
来源：http://qoa.xuanzx.com

[F01] 读取整个文件
来源：http://rlp.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kxj.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://wob.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bzd.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jpn.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://lkp.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ecd.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://why.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://mxe.hammf.cn

[F02] 逐行读取文件
来源：http://ept.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ffq.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aea.0kj1m.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dkc.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egz.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dzz.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mij.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bgh.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gli.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://pez.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tbq.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://exa.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bjy.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwq.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rbp.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zjx.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://yay.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ilj.uphjek.com

[F04] 追加写入文件
来源：http://anp.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yxy.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dqv.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ywk.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tyw.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qkx.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nyt.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hub.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pdp.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://mwl.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pbw.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://onq.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://bpf.hysaishi.cn

TS:   fs.existsSync("a.txt")
来源：http://bnb.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dxs.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://teh.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://vng.ywan-chungtsiang.top


<!-- 参考信息 -->