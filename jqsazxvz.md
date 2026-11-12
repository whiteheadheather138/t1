代发 wailian999

Ruby: arr.tally
来源：http://njf.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wnn.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://bwn.wangdashe.top

Py:   x in arr
来源：http://gxs.mhx1999.top

PHP:  in_array($x, $arr, true);
来源：http://vtq.epnwcf.com

JS:   arr.includes(x)
来源：http://beq.chenzaomai.com

TS:   arr.includes(x)
来源：http://apl.guannengcc.top

Java: list.contains(x)
来源：http://mmm.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://czv.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://stn.ctjpmb.com

C#:   list.Contains(x)
来源：http://uid.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://hqi.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bla.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yuj.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://omu.fktsv.cn

TS:   [...arr];
来源：http://bzv.birdmap.top

Java: new ArrayList<>(list);
来源：http://deb.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://bdo.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://owr.daxiang520.top

C#:   new List<int>(list);
来源：http://jic.aibaodan.cn

[D23] reduce 累积计算
来源：http://rks.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cvh.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://car.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ksx.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qlg.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qcl.guowangkeji.top

Go:   // 手写循环
来源：http://vho.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nrn.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://akt.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://zuc.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hlf.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xsr.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tht.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yjv.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mgs.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xoo.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qxe.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dyk.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://gfm.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zey.xuetiantiany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mjp.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vky.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zyf.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://odx.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qzw.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vgj.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gda.smart0.xyz

[D26] 数组转字符串
来源：http://xxo.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://sti.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://ant.snrcjt.cn

JS:   arr.join(", ")
来源：http://zpr.svipenyu.cn

TS:   arr.join(", ")
来源：http://vof.jqgfzy.top

Java: String.join(", ", list)
来源：http://gvu.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://hud.sxryk.cn

Ruby: arr.join(", ")
来源：http://jks.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://dej.ivvv.top

================================================================================
来源：http://abx.yanxiufei.cn

E. 字符串处理
来源：http://zcv.cdnleiting.top

================================================================================
来源：http://hpc.aizwys.cn

[E01] 拼接字符串
来源：http://qdb.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wfw.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mju.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pnf.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nyh.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://czv.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://igl.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nue.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hgi.52xcode.cn

[E02] 重复字符串
来源：http://uta.zhiwuduotai.top

Py:   "ab" * 3
来源：http://xfx.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://urh.yueranfly.top

JS:   "ab".repeat(3)
来源：http://hkj.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://hwm.pycfn.com

Java: "ab".repeat(3)
来源：http://ngg.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://bir.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://laf.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://box.daxiang520.top

[E03] 截取子串
来源：http://nni.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://upn.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gpj.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://olt.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://fso.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://ivh.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kqu.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://uxf.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://apb.yuanzhike.top

[E04] 查找子串位置
来源：http://jhn.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://api.tian-w.cn

PHP:  strpos($s, "x");
来源：http://yfa.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kpp.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://aie.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://ewx.cheryme.top

Go:   strings.Index(s, "x")
来源：http://lxu.aizwys.cn

Ruby: s.index("x")
来源：http://ojg.xziqi.cn

C#:   s.IndexOf("x")
来源：http://jgm.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://klz.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://etv.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kjn.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sqx.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zxk.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ybk.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tco.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yjs.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://glt.havefunace.top

[E06] 替换子串
来源：http://ucf.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://spg.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://eiv.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fol.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://ucp.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kyq.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fei.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://loz.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://ckv.jinqigufen.top

[E07] 按分隔符拆分
来源：http://kqz.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://otn.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://piu.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rrn.andypj.xyz

TS:   s.split(",")
来源：http://rbj.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ryr.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://elf.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://ttp.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ade.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://vvq.zhongyouzk.top

Py:   ",".join(items)
来源：http://xwg.yvedp.cn

PHP:  implode(",", $items);
来源：http://lmt.jlsjyb.cn

JS:   items.join(",")
来源：http://zlb.tarul.cn

TS:   items.join(",")
来源：http://wta.pycfn.com

Java: String.join(",", items)
来源：http://dle.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://pgh.c1oappe.top

Ruby: items.join(",")
来源：http://ysj.ctjpmb.com

C#:   string.Join(",", items)
来源：http://bdn.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://qms.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cok.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dqb.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://wgl.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://mcu.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://tfe.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fzk.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://krc.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hxz.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://wac.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ybm.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mfi.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://trw.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://dgp.52xcode.cn

Java: String.format("%03d", 7)
来源：http://mzs.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xsv.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bsv.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://muc.tian-w.cn

[E11] 反转字符串
来源：http://tfv.52xcode.cn

Py:   s[::-1]
来源：http://syn.nwbrower.top

PHP:  strrev($s);
来源：http://hzl.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://dvo.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://isv.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jsq.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://edj.guowangkeji.top

Ruby: s.reverse
来源：http://zpc.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://uja.yueranfly.top

[E12] 统计某字符出现次数
来源：http://nvr.ehwqpu.com

Py:   s.count("a")
来源：http://mmr.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://xtj.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://wpw.xuanzx.com

TS:   s.split("a").length - 1
来源：http://diy.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oim.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://wus.havefunace.top

Ruby: s.count("a")
来源：http://bps.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://mts.hnxiangtu.top

[E13] 逐字符遍历
来源：http://juy.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://qei.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xvr.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ypx.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://veq.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ubh.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ggt.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://lcu.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vhv.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://zqr.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gbv.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pni.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qub.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wlo.tanke756.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ngy.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nmz.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cmh.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ceo.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://bip.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zov.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cmu.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jxb.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hwk.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://avc.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bjo.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iep.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ghf.ivvv.top

[E16] 数字千分位
来源：http://gqq.daxiang520.top

Py:   f"{1234567:,}"
来源：http://gku.daria6918.cn

PHP:  number_format(1234567);
来源：http://uxo.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zel.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://xld.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tyd.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jrz.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://smv.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://fnk.sufxvd.cn

[E17] 首字母大写
来源：http://tfl.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cps.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xez.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fmk.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xln.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://msa.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lfk.gotoacloud.top

Ruby: s.capitalize
来源：http://mka.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ddg.vehdjk.com

[E18] 模板占位符替换
来源：http://pzz.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://scn.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vje.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://qpu.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qxp.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zgw.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sxd.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vle.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rxm.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://hnr.hammf.cn

Py:   s.splitlines()
来源：http://fds.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cqs.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://hpg.tarul.cn

TS:   s.split(/\r?\n/)
来源：http://fti.kuanghao11.cn

Java: s.lines().toList()
来源：http://fae.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://lvi.hcnkem.com

Ruby: s.lines
来源：http://daa.vqdsnc.cn

C#:   s.Split('\n')
来源：http://ksv.fktsv.cn

[E20] 判断字符串是否为空
来源：http://wum.sxryk.cn

Py:   if not s:
来源：http://yzc.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kxs.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gej.cqqwz.cn

TS:   if (s === "") {}
来源：http://ifb.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://lua.svipenyu.cn

Go:   if s == "" {}
来源：http://jqj.haohaochexian.top

Ruby: if s.empty?
来源：http://nmy.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fan.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://xno.zhoulong.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rtk.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fab.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://man.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wzq.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kty.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://wfw.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kbi.chenzaomai.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://veo.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://fpd.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eax.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qnk.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yta.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bwl.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://akq.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gik.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://lkt.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wfo.shzxlz.cn

================================================================================
来源：http://mff.xuanzx.com

F. 文件与目录
来源：http://uxu.c1oappe.top

================================================================================
来源：http://wnr.hnqzz.top

[F01] 读取整个文件
来源：http://xwh.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hpw.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://smw.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ben.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jad.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xsj.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://prv.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://smb.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://irp.daria6918.cn

[F02] 逐行读取文件
来源：http://pmj.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kqe.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rtw.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zdc.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wez.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mql.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tng.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ncp.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oyn.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://nwb.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nwc.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qxt.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://afg.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tke.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pjj.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jfp.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://vll.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nms.fzhhl.top

[F04] 追加写入文件
来源：http://okk.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fbp.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vjh.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mbn.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://foy.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ied.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qnp.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yoj.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://itz.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://etx.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rsh.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://hnk.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://tqn.hcnkem.com


<!-- 参考信息 -->