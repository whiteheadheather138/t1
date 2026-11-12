代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cjw.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://tlp.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pdw.gogol.net.cn

TS:   nested.flat();
来源：http://lwj.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gcz.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://qnh.dashuyun.cn

Ruby: nested.flatten
来源：http://mby.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mfi.zdqjudy.top

[D19] 按字段分组
来源：http://sud.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nms.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://emc.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qvp.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://enh.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://heg.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://wao.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ujo.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ufa.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://nvt.hcnkem.com

Py:   Counter(arr)
来源：http://urg.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://pzj.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qki.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gft.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hzb.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://rku.birdmap.top

Ruby: arr.tally
来源：http://nyw.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://afg.fzhhl.top

[D21] 判断是否包含某元素
来源：http://wet.tarul.cn

Py:   x in arr
来源：http://ixa.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://soy.havefunace.top

JS:   arr.includes(x)
来源：http://aso.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://fzq.fktsv.cn

Java: list.contains(x)
来源：http://ish.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://pfz.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://psb.hfpthk.cn

C#:   list.Contains(x)
来源：http://epx.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://jsi.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wzt.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gnp.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wvh.iojbl.cn

TS:   [...arr];
来源：http://xuk.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://ijx.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://mwr.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://nuu.hnxiangtu.top

C#:   new List<int>(list);
来源：http://ulc.shuidangran.top

[D23] reduce 累积计算
来源：http://ztk.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://olz.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aeo.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oak.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xpf.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nmf.pengpengdd.cyou

Go:   // 手写循环
来源：http://ozk.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ihp.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tdy.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://gxv.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://prw.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nne.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dlk.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zzt.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cvk.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qli.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lmz.cdnleiting.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aac.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://led.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cev.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kpf.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aya.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xop.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lzu.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ilw.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xfu.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gij.yongpay.top

[D26] 数组转字符串
来源：http://jvx.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://kcp.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://vlb.ehwqpu.com

JS:   arr.join(", ")
来源：http://gpi.nanxuanxn.top

TS:   arr.join(", ")
来源：http://msx.sysykeji.top

Java: String.join(", ", list)
来源：http://uzx.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://hkk.zhixingplan.top

Ruby: arr.join(", ")
来源：http://cey.xuanzx.com

C#:   string.Join(", ", list)
来源：http://qav.yuxming.cn

================================================================================
来源：http://mxm.chenjidiqi.icu

E. 字符串处理
来源：http://jja.jiagoushi.top

================================================================================
来源：http://doy.smart0.xyz

[E01] 拼接字符串
来源：http://laa.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wpf.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wbh.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dey.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lzs.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://etz.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ghq.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ejs.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vzi.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://ean.zhiwuduotai.top

Py:   "ab" * 3
来源：http://dsz.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://lak.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://yuv.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://gef.xinyue.icu

Java: "ab".repeat(3)
来源：http://wlm.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://zzp.hesvh.cn

Ruby: "ab" * 3
来源：http://uts.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://amu.xuetiantiany.cn

[E03] 截取子串
来源：http://ndj.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ynq.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rzx.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hdp.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://txk.meibo888.top

Java: s.substring(1, 4)
来源：http://zzi.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kmh.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://tmq.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://pih.ivvv.top

[E04] 查找子串位置
来源：http://jms.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://dmv.yueranfly.top

PHP:  strpos($s, "x");
来源：http://rgz.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ded.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://qsr.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://gsp.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://vpb.zycfv.cn

Ruby: s.index("x")
来源：http://nfp.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://rws.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nss.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kjp.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dgm.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zuv.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fmn.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oqn.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tke.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qja.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wkp.fktsv.cn

[E06] 替换子串
来源：http://mbg.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pxv.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://rbu.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://awz.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://luu.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ulw.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cxn.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lwu.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://epi.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://ten.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sym.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gvp.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wie.hongshengwenyu.top

TS:   s.split(",")
来源：http://hbq.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wbe.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qsz.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://auy.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://whq.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://aur.xuanzx.com

Py:   ",".join(items)
来源：http://ips.yj202588.top

PHP:  implode(",", $items);
来源：http://hri.quarkkingdee.top

JS:   items.join(",")
来源：http://dbb.hongshengwenyu.top

TS:   items.join(",")
来源：http://hcr.zhiwuduotai.top

Java: String.join(",", items)
来源：http://axk.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://kfe.quarkkingdee.top

Ruby: items.join(",")
来源：http://xad.316326.xyz

C#:   string.Join(",", items)
来源：http://tmw.yfazqb.com

[E09] 去除所有空白字符
来源：http://fdi.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aye.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nwp.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://qhd.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://axz.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://eyj.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kvx.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://yix.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gbm.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://zck.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://njd.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qmj.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://vae.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://eoh.pycfn.com

Java: String.format("%03d", 7)
来源：http://orf.guannengcc.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://oum.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rwa.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lnh.wangdashe.top

[E11] 反转字符串
来源：http://iwt.fzhhl.top

Py:   s[::-1]
来源：http://afz.9152youxi.cn

PHP:  strrev($s);
来源：http://jvt.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://nvx.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://iiw.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vrc.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xxo.zdqjudy.top

Ruby: s.reverse
来源：http://mhx.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://skk.ydzc1.top

[E12] 统计某字符出现次数
来源：http://gga.hnqzz.top

Py:   s.count("a")
来源：http://yps.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://kyv.yonumen.top

JS:   s.split("a").length - 1
来源：http://kzg.guannengcc.top

TS:   s.split("a").length - 1
来源：http://tdm.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://niv.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://fsy.shangyingyoupin.top

Ruby: s.count("a")
来源：http://tte.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://msa.yj202588.top

[E13] 逐字符遍历
来源：http://pas.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://rfg.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ecy.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://fzw.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hdc.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ihg.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nbt.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dxe.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://emj.yongpay.top

[E14] URL 编码与 Base64
来源：http://vkf.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rtq.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dwz.vqdsnc.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vpa.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gzb.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xuc.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rsc.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uof.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rdo.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://fty.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uky.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://emu.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jgi.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bsq.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://edb.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ttw.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ruf.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://czg.zdqjudy.top

[E16] 数字千分位
来源：http://lfb.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://zjm.redwolf501.top

PHP:  number_format(1234567);
来源：http://xcs.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ckk.zdqjudy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nwc.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ypc.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gup.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://szd.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://dah.sjlbkw.cn

[E17] 首字母大写
来源：http://uzj.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://drj.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jbl.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qnb.nwbrower.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dec.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://trj.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ppx.svipenyu.cn

Ruby: s.capitalize
来源：http://set.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nif.ydjk.org.cn

[E18] 模板占位符替换
来源：http://zxb.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gzm.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zxz.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kfu.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zad.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wcl.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://idl.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://csk.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://haw.bbcook.cn

[E19] 多行文本按行拆分
来源：http://yot.uphjek.com

Py:   s.splitlines()
来源：http://jdw.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dms.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://jxl.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://vuz.zhengqikj.top

Java: s.lines().toList()
来源：http://byz.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://vcq.chenlongwang.top

Ruby: s.lines
来源：http://zqu.fktsv.cn

C#:   s.Split('\n')
来源：http://fal.epnwcf.com

[E20] 判断字符串是否为空
来源：http://qld.jinqigfzy.top

Py:   if not s:
来源：http://mrl.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zgc.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://esu.hfpthk.cn

TS:   if (s === "") {}
来源：http://xog.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://vlo.ydzc1.top

Go:   if s == "" {}
来源：http://llr.ctjpmb.com

Ruby: if s.empty?
来源：http://acc.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ojr.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://ypq.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rbz.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lqk.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qqr.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://szw.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qeo.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://zte.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://djz.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://net.ybcxt.top

[E22] 字节长度与字符长度
来源：http://zpv.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rsy.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ses.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jbm.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kod.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sah.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://evq.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://bhq.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tdn.xuetiantiany.cn

================================================================================
来源：http://hvq.nanxinkj.top

F. 文件与目录
来源：http://lgg.gaohongyu789.top

================================================================================
来源：http://epl.dianchejie.cn

[F01] 读取整个文件
来源：http://lbl.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nwp.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://vdn.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mos.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gdr.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oud.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mim.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://xbj.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://cov.xuanzx.com

[F02] 逐行读取文件
来源：http://ijr.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zxl.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pif.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vqb.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rji.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kvu.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dwc.hcnkem.com


<!-- 参考信息 -->