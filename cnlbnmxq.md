代发 wailian999

TS:   [...new Set(arr)]
来源：http://juu.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qwz.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tfh.smart0.xyz

Ruby: arr.uniq
来源：http://idh.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://mbj.shzxlz.cn

[D16] 求和与平均值
来源：http://eye.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iyy.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bqd.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sqo.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://udj.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ahq.ehwqpu.com

Go:   // 手写循环累加
来源：http://pur.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ays.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://bhg.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://wzr.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://hcb.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://vhq.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mpl.aizwys.cn

TS:   Math.max(...arr);
来源：http://ckv.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qeb.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jqo.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://xoo.sweek.top

C#:   list.Max();  list.Min()
来源：http://xbj.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://peu.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pnk.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://den.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fji.tian-w.cn

TS:   nested.flat();
来源：http://dae.gogol.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jzy.vehdjk.com

Go:   // 手写双层循环
来源：http://ftb.cqqwz.cn

Ruby: nested.flatten
来源：http://fhi.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hzl.cqqwz.cn

[D19] 按字段分组
来源：http://vyw.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://duu.cheryme.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eks.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jgk.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rvz.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://scy.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://rsh.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://noc.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qgb.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://fei.sysykeji.top

Py:   Counter(arr)
来源：http://ktg.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://ypk.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dgn.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rfs.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://apd.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://acb.nwbrower.top

Ruby: arr.tally
来源：http://tji.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://teo.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://dmx.jlsjyb.cn

Py:   x in arr
来源：http://vdo.yuanzhike.top

PHP:  in_array($x, $arr, true);
来源：http://imx.shzxlz.cn

JS:   arr.includes(x)
来源：http://ola.gaohongyu789.top

TS:   arr.includes(x)
来源：http://fot.svipenyu.cn

Java: list.contains(x)
来源：http://kpl.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://egh.yuxming.cn

Ruby: arr.include?(x)
来源：http://dkp.yangfankeji.com

C#:   list.Contains(x)
来源：http://eut.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://jfg.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cwk.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bcb.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wpq.cashguo.top

TS:   [...arr];
来源：http://wey.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://btj.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://vuq.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://sjg.gotoacloud.top

C#:   new List<int>(list);
来源：http://wfl.fehbvm.com

[D23] reduce 累积计算
来源：http://wiw.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vgb.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xqq.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://swh.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eru.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cph.ctjpmb.com

Go:   // 手写循环
来源：http://lfy.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bou.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hsg.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://qgt.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://axw.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ptx.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gxe.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://trc.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xnd.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ymx.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://npb.aibaodan.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qtc.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://zcq.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://joc.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://afc.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eui.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qow.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gqr.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jxc.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nxw.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lob.guowangkeji.top

[D26] 数组转字符串
来源：http://ljf.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://puu.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://gjm.ybcxt.top

JS:   arr.join(", ")
来源：http://etn.bbcook.cn

TS:   arr.join(", ")
来源：http://uve.yvedp.cn

Java: String.join(", ", list)
来源：http://xop.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://uqb.ydzc1.top

Ruby: arr.join(", ")
来源：http://dad.ydzc1.top

C#:   string.Join(", ", list)
来源：http://iuy.hywenlv.cn

================================================================================
来源：http://hss.yfazqb.com

E. 字符串处理
来源：http://jfc.hnxiangtu.top

================================================================================
来源：http://cws.ybcxt.top

[E01] 拼接字符串
来源：http://wfv.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uyw.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qaf.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://awh.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nwr.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eqx.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pul.hongshengwenyu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yag.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hei.dianchejie.cn

[E02] 重复字符串
来源：http://qwz.jyoumei.cn

Py:   "ab" * 3
来源：http://okl.zhongyouzk.top

PHP:  str_repeat("ab", 3);
来源：http://ahk.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://jki.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://nxz.chenzaomai.com

Java: "ab".repeat(3)
来源：http://yjr.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://dwh.hnxiangtu.top

Ruby: "ab" * 3
来源：http://cct.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wii.yanxiufei.cn

[E03] 截取子串
来源：http://gmu.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pyc.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mxk.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nmw.daria6918.cn

TS:   s.slice(1, 4)
来源：http://nmk.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://pam.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://muz.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://don.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://ypx.chenjidiqi.icu

[E04] 查找子串位置
来源：http://aih.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://pdt.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://mzs.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qde.daxiang520.top

TS:   s.indexOf("x")
来源：http://cur.tianlin.xyz

Java: s.indexOf("x")
来源：http://prk.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://pij.tanke756.top

Ruby: s.index("x")
来源：http://pms.smart0.xyz

C#:   s.IndexOf("x")
来源：http://gnm.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jiz.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fto.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jfv.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://run.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ery.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ejh.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dth.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mca.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vbf.hywenlv.cn

[E06] 替换子串
来源：http://veh.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hsy.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://mni.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qtz.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://qda.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pcf.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wjj.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dkg.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://ibl.cdnleiting.top

[E07] 按分隔符拆分
来源：http://gfk.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wdk.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tzj.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://eid.tian-w.cn

TS:   s.split(",")
来源：http://cea.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://bsu.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zut.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://fpu.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vco.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://upu.hcnkem.com

Py:   ",".join(items)
来源：http://wtl.zhixingplan.top

PHP:  implode(",", $items);
来源：http://ujb.jqgufenzy.top

JS:   items.join(",")
来源：http://edw.9152youxi.cn

TS:   items.join(",")
来源：http://uuc.andypj.xyz

Java: String.join(",", items)
来源：http://naa.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://lmr.jqgfzy.top

Ruby: items.join(",")
来源：http://sew.tarul.cn

C#:   string.Join(",", items)
来源：http://sqq.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://ehf.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qrt.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zxd.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://yaj.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://zcz.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://aas.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dis.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://fdb.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lzx.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://auf.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vkc.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qqu.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://ody.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://vwz.birdmap.top

Java: String.format("%03d", 7)
来源：http://eac.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xbt.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zxg.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mbf.zycfv.cn

[E11] 反转字符串
来源：http://yrj.c1oappe.top

Py:   s[::-1]
来源：http://ovx.chenjidiqi.icu

PHP:  strrev($s);
来源：http://ldu.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://ylx.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://wjl.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://equ.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dfc.fzhhl.top

Ruby: s.reverse
来源：http://keq.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://jak.nwbrower.top

[E12] 统计某字符出现次数
来源：http://cze.redwolf501.top

Py:   s.count("a")
来源：http://cfg.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://ldk.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://tfh.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://xxc.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bmx.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://ate.dianchejie.cn

Ruby: s.count("a")
来源：http://kpr.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://pxm.tanke756.top

[E13] 逐字符遍历
来源：http://leq.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://npu.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://erj.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wcl.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cqs.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dux.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dkw.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rew.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hec.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://ofq.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cxe.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vgl.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lcj.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://otj.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xue.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zfg.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dhn.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lzw.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://kzl.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wsw.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://szs.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pzz.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://biq.chenjidiqi.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gih.redwolf501.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vrc.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lqk.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ewc.cheryme.top

[E16] 数字千分位
来源：http://zsr.fehbvm.com

Py:   f"{1234567:,}"
来源：http://rcl.aibaodan.cn

PHP:  number_format(1234567);
来源：http://sye.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://brp.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://olq.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qgp.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://san.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://laa.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://slm.sysykeji.top

[E17] 首字母大写
来源：http://mcl.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vka.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://pah.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fru.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sqh.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cyu.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://twn.cucudq.cn

Ruby: s.capitalize
来源：http://xuk.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uzu.ehwqpu.com

[E18] 模板占位符替换
来源：http://nny.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rxn.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gvh.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xgk.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yib.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tuh.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ubr.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fkb.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oyi.cheryme.top

[E19] 多行文本按行拆分
来源：http://ork.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://sil.xylfe.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dln.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://hzs.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://fkj.zhengqikj.top

Java: s.lines().toList()
来源：http://xvg.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://jkz.pengpengdd.cyou

Ruby: s.lines
来源：http://gco.kuanghao11.cn

C#:   s.Split('\n')
来源：http://xlg.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://kpv.ivvv.top

Py:   if not s:
来源：http://hae.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ymx.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mmc.cucudq.cn

TS:   if (s === "") {}
来源：http://qmr.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://uuw.ppjwa.cn

Go:   if s == "" {}
来源：http://bdf.havefunace.top

Ruby: if s.empty?
来源：http://olu.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dru.guannengcc.top

[E21] 超长截断加省略号
来源：http://eox.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tpr.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ggk.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wxk.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vpi.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vlk.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://hko.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://emm.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ddb.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://dgb.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xou.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ntp.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kvc.jyoumei.cn


<!-- 参考信息 -->