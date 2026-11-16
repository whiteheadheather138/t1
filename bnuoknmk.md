代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nye.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blo.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nru.bbcook.cn

Go:   // 手写 map[T]int
来源：http://azi.xuanzx.com

Ruby: arr.tally
来源：http://pij.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mtt.yonumen.top

[D21] 判断是否包含某元素
来源：http://vfb.ehwqpu.com

Py:   x in arr
来源：http://gct.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://dat.hysaishi.cn

JS:   arr.includes(x)
来源：http://kci.zhixingplan.top

TS:   arr.includes(x)
来源：http://ehl.yanxiufei.cn

Java: list.contains(x)
来源：http://hao.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://pof.shuidangran.top

Ruby: arr.include?(x)
来源：http://lpq.jinqigufen.top

C#:   list.Contains(x)
来源：http://bjj.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://dnr.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://djh.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tvn.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mve.fehbvm.com

TS:   [...arr];
来源：http://jbc.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://snm.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wlg.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://tdh.gogol.net.cn

C#:   new List<int>(list);
来源：http://xya.chenzaomai.com

[D23] reduce 累积计算
来源：http://cvt.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rgj.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ypq.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://esd.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hyb.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hvn.redwolf501.top

Go:   // 手写循环
来源：http://pbq.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wua.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oym.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://dfl.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://chr.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xjw.nanxinkj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xsk.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sfc.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://him.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fsi.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xdd.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wkv.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://imm.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ccy.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://csy.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yvr.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rkq.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://afz.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yxt.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sqc.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vrf.jqgufenzy.top

[D26] 数组转字符串
来源：http://dkj.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://uog.yongpay.top

PHP:  implode(", ", $arr);
来源：http://nem.chenjidiqi.icu

JS:   arr.join(", ")
来源：http://ycg.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://drk.ivvv.top

Java: String.join(", ", list)
来源：http://wkz.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://mie.nwbrower.top

Ruby: arr.join(", ")
来源：http://ifm.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://deu.gaohongyu789.top

================================================================================
来源：http://aka.jqgufenzy.top

E. 字符串处理
来源：http://kyj.52xcode.cn

================================================================================
来源：http://ljx.smart0.xyz

[E01] 拼接字符串
来源：http://tzd.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hyu.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uyo.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pdq.zycfv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xts.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bjc.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://omo.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://isr.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mxt.hongshengwenyu.top

[E02] 重复字符串
来源：http://fzy.xuetiantiany.cn

Py:   "ab" * 3
来源：http://ktz.pycfn.com

PHP:  str_repeat("ab", 3);
来源：http://owl.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://dzx.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://mbr.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://lxx.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://chi.gzhubu.top

Ruby: "ab" * 3
来源：http://uiz.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pkk.zdbjq.cn

[E03] 截取子串
来源：http://nvr.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eos.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cmg.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bcf.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://juh.jianghu66.top

Java: s.substring(1, 4)
来源：http://ncb.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zpm.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vdg.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://asq.ybcxt.top

[E04] 查找子串位置
来源：http://lwq.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://kjs.yj202588.top

PHP:  strpos($s, "x");
来源：http://vpq.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jqu.ydzc1.top

TS:   s.indexOf("x")
来源：http://xgi.guannengcc.top

Java: s.indexOf("x")
来源：http://ocy.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://jze.yuanzhike.top

Ruby: s.index("x")
来源：http://jml.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://jxo.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zci.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nkt.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wzm.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jer.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://els.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rgk.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zqr.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wke.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xwo.andypj.xyz

[E06] 替换子串
来源：http://dgd.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://njw.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://adm.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vwa.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://jqc.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iai.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tdh.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vll.aibaodan.cn

C#:   s.Replace("a", "b")
来源：http://yjc.dianchejie.cn

[E07] 按分隔符拆分
来源：http://ntx.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pbk.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bqz.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iyh.yuanzhike.top

TS:   s.split(",")
来源：http://yid.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://uoc.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lob.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://sdq.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xdh.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://knt.ctjpmb.com

Py:   ",".join(items)
来源：http://wom.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://hrf.zycfv.cn

JS:   items.join(",")
来源：http://ral.hnqzz.top

TS:   items.join(",")
来源：http://dcz.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://ooq.gogol.net.cn

Go:   strings.Join(items, ",")
来源：http://kys.dashuyun.cn

Ruby: items.join(",")
来源：http://deh.jyoumei.cn

C#:   string.Join(",", items)
来源：http://hro.52xcode.cn

[E09] 去除所有空白字符
来源：http://odq.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oim.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uhi.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://iav.aizwys.cn

TS:   s.replace(/\s+/g, "")
来源：http://nup.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://fkp.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nzw.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://afd.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://arh.jinqigufen.top

[E10] 左侧补零 / 定长填充
来源：http://cxo.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wpm.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ezq.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://dve.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://emu.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://mrk.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://noc.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dou.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xsu.ivvv.top

[E11] 反转字符串
来源：http://nsm.yvedp.cn

Py:   s[::-1]
来源：http://jhj.hammf.cn

PHP:  strrev($s);
来源：http://ybk.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://wrd.cashguo.top

TS:   [...s].reverse().join("")
来源：http://wlh.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yky.jinqigfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nbw.fktsv.cn

Ruby: s.reverse
来源：http://dsc.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://tpu.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://dmd.hywenlv.cn

Py:   s.count("a")
来源：http://xhu.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://kxg.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://xxi.jianghu66.top

TS:   s.split("a").length - 1
来源：http://pvs.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://npf.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://vhu.andypj.xyz

Ruby: s.count("a")
来源：http://hau.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://bgl.zhixingplan.top

[E13] 逐字符遍历
来源：http://cbf.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://vbd.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vom.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iuz.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yyv.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lsu.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dmm.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zvn.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bix.meibo888.top

[E14] URL 编码与 Base64
来源：http://swe.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://smp.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zmm.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://icg.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://riy.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jnb.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ful.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qkb.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jrg.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://qeg.jyoumei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lfg.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sjc.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://spw.redwolf501.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pzr.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ghe.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://glr.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jiw.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gzh.hammf.cn

[E16] 数字千分位
来源：http://jby.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://gsc.iojbl.cn

PHP:  number_format(1234567);
来源：http://wpy.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://dbw.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pvp.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://myu.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dkg.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qao.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://wea.sweek.top

[E17] 首字母大写
来源：http://ezz.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nyz.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vlc.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dto.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzd.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ria.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://crm.wangdashe.top

Ruby: s.capitalize
来源：http://idf.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rhs.tianlin.xyz

[E18] 模板占位符替换
来源：http://wap.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hxv.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vgz.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oqi.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oke.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zyp.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ocz.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lcy.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ztp.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://gsy.vqdsnc.cn

Py:   s.splitlines()
来源：http://psd.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rus.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://mgw.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://uod.bjfxy.top

Java: s.lines().toList()
来源：http://fir.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://ynl.mhx1999.top

Ruby: s.lines
来源：http://orf.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://yva.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://ldw.hnqzz.top

Py:   if not s:
来源：http://iae.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bvl.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ypb.zhijiandao.cn

TS:   if (s === "") {}
来源：http://cjx.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://vab.jinqigfzy.top

Go:   if s == "" {}
来源：http://iig.ydzc1.top

Ruby: if s.empty?
来源：http://rwz.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qsq.zhixingplan.top

[E21] 超长截断加省略号
来源：http://gpm.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gsg.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nis.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qcw.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ncu.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rcm.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://oua.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yjp.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gms.fktsv.cn

[E22] 字节长度与字符长度
来源：http://oxu.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ivq.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oxx.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mqh.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://krj.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ykh.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ofy.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://jbp.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vsa.kuanghao11.cn

================================================================================
来源：http://jzo.guowangkeji.top

F. 文件与目录
来源：http://zbc.daria6918.cn

================================================================================
来源：http://rgi.daxiang520.top

[F01] 读取整个文件
来源：http://ina.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vmu.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://nkb.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://inz.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://smt.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yvi.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fio.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://njs.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://jdn.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://rru.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ojp.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zrz.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hal.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://okg.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kas.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jzv.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nka.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lnn.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://fcc.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gme.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://maz.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tjr.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jgh.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uey.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xpd.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://vqc.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fcy.hnxiangtu.top

[F04] 追加写入文件
来源：http://jnz.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wqe.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oyv.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uur.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vta.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dsb.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://acw.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://asc.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bia.shanyushiyangkeji.top


<!-- 参考信息 -->