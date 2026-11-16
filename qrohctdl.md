代发 wailian999

TS:   [...new Set(arr)]
来源：http://hra.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uoi.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://gvs.hcnkem.com

Ruby: arr.uniq
来源：http://arn.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://wus.tian-w.cn

[D16] 求和与平均值
来源：http://cto.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ejj.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rbv.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://exm.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dey.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cpv.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://hfz.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bgv.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://gif.havefunace.top

[D17] 最大值与最小值
来源：http://vkw.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://wfk.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://bez.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qey.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://kbj.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ztk.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ecx.cheryme.top

Ruby: arr.max;  arr.min
来源：http://uud.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://clq.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://mxj.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://egi.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://xtf.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cfy.gotoacloud.top

TS:   nested.flat();
来源：http://wbn.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://knt.chenzaomai.com

Go:   // 手写双层循环
来源：http://edo.yfazqb.com

Ruby: nested.flatten
来源：http://rmc.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://dic.ppjwa.cn

[D19] 按字段分组
来源：http://gin.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ppi.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cbm.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zwx.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://koh.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cbb.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://aza.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rei.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iww.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://ziy.sweek.top

Py:   Counter(arr)
来源：http://rzy.hesvh.cn

PHP:  array_count_values($arr);
来源：http://dlz.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxm.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ifw.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://svq.52xcode.cn

Go:   // 手写 map[T]int
来源：http://jld.chenlongwang.top

Ruby: arr.tally
来源：http://yfz.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gog.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://sys.hywenlv.cn

Py:   x in arr
来源：http://tgb.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://eow.hywenlv.cn

JS:   arr.includes(x)
来源：http://rww.yvedp.cn

TS:   arr.includes(x)
来源：http://sbo.cheryme.top

Java: list.contains(x)
来源：http://wpm.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://gqr.fehbvm.com

Ruby: arr.include?(x)
来源：http://zna.smart0.xyz

C#:   list.Contains(x)
来源：http://yts.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://wpb.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://osk.fanxiaobao.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iri.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://unr.ppjwa.cn

TS:   [...arr];
来源：http://lqk.daxiang520.top

Java: new ArrayList<>(list);
来源：http://dqy.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pep.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://tir.hnxiangtu.top

C#:   new List<int>(list);
来源：http://kuo.bbcook.cn

[D23] reduce 累积计算
来源：http://wft.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cuq.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jos.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ehh.bjfxy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ria.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ooe.cucudq.cn

Go:   // 手写循环
来源：http://xeq.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rsf.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mnw.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://ore.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zzy.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qpg.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gdb.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pgh.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://usb.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jct.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gjx.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://chn.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://sza.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tio.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lel.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mic.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tix.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cqs.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ihl.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vuu.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://btf.zdqjudy.top

[D26] 数组转字符串
来源：http://nsk.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://oso.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://usv.52xcode.cn

JS:   arr.join(", ")
来源：http://nlu.fktsv.cn

TS:   arr.join(", ")
来源：http://qnh.zdbjq.cn

Java: String.join(", ", list)
来源：http://hya.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://wgg.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://bvx.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://qrz.316326.xyz

================================================================================
来源：http://mil.svipenyu.cn

E. 字符串处理
来源：http://xoy.hnqzz.top

================================================================================
来源：http://vus.dianchejie.cn

[E01] 拼接字符串
来源：http://bgl.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ykw.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bff.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://biw.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://toi.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ltm.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dop.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rnn.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cfo.dashuyun.cn

[E02] 重复字符串
来源：http://zkz.wangshuangyany.cn

Py:   "ab" * 3
来源：http://jzs.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://dje.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://rgu.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://lmg.yuanzhike.top

Java: "ab".repeat(3)
来源：http://zgb.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://uyj.yonumen.top

Ruby: "ab" * 3
来源：http://xal.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gvz.jinqigufen.top

[E03] 截取子串
来源：http://igu.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ett.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qtj.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mpy.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://egp.cdnleiting.top

Java: s.substring(1, 4)
来源：http://jyh.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uud.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://fjm.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://vnl.zhengqikj.top

[E04] 查找子串位置
来源：http://zbr.hnxiangtu.top

Py:   s.find("x");  s.index("x")
来源：http://rvq.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://oko.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lff.yj20258.top

TS:   s.indexOf("x")
来源：http://epe.wangdashe.top

Java: s.indexOf("x")
来源：http://iir.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://dcl.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://uez.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://kke.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://itm.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zyj.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xmy.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dqq.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yqi.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lpu.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uki.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hwb.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mft.hesvh.cn

[E06] 替换子串
来源：http://arl.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qtj.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://zdb.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cor.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://pfo.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lld.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dpl.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fch.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://rzg.svipenyu.cn

[E07] 按分隔符拆分
来源：http://xpx.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://brr.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bhl.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mzo.gogol.net.cn

TS:   s.split(",")
来源：http://ogp.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qmn.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qkk.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://uac.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://khq.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://nwo.tianlin.xyz

Py:   ",".join(items)
来源：http://iul.yj202588.top

PHP:  implode(",", $items);
来源：http://qgl.jinghuilouyu.cn

JS:   items.join(",")
来源：http://dfd.tianlin.xyz

TS:   items.join(",")
来源：http://iaj.zycfv.cn

Java: String.join(",", items)
来源：http://iug.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://ubw.jyoumei.cn

Ruby: items.join(",")
来源：http://qpg.yj20258.top

C#:   string.Join(",", items)
来源：http://dyc.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://ref.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fmx.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yxl.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://osl.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://vcb.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://pti.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cmz.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://imf.hfpthk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ycq.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://dct.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xoc.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://val.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://ski.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://smp.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://vnw.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ipa.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dex.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qiy.sweek.top

[E11] 反转字符串
来源：http://nui.chenlongwang.top

Py:   s[::-1]
来源：http://lfi.vehdjk.com

PHP:  strrev($s);
来源：http://ecx.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://cbe.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://zuq.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ahc.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ghu.pengpengdd.cyou

Ruby: s.reverse
来源：http://bfm.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://swp.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://xyb.nanxuanxn.top

Py:   s.count("a")
来源：http://cbx.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://qei.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://elc.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://jld.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rjz.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://xiu.yuxming.cn

Ruby: s.count("a")
来源：http://bey.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://sgy.yvedp.cn

[E13] 逐字符遍历
来源：http://sjp.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://kza.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://srr.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kgr.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gpt.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://moj.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://atj.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://gqy.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://koz.hnqzz.top

[E14] URL 编码与 Base64
来源：http://pho.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ucp.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uty.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dsl.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mqz.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pzu.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fhz.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vop.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ora.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://yea.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dmi.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bjp.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mks.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ive.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qcw.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iyp.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pay.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rpb.zycfv.cn

[E16] 数字千分位
来源：http://ynf.havefunace.top

Py:   f"{1234567:,}"
来源：http://lmp.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://uzw.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wjx.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qef.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zrx.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://prm.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ofi.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://gij.epnwcf.com

[E17] 首字母大写
来源：http://ixu.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oaa.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://abj.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://khw.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://znq.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gsm.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ntx.hongshengwenyu.top

Ruby: s.capitalize
来源：http://ieg.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qni.zhoulong.xyz

[E18] 模板占位符替换
来源：http://xmh.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yic.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yxz.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bcp.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wiz.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qok.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nun.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aru.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ilh.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://wcq.quarkkingdee.top

Py:   s.splitlines()
来源：http://ccn.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ypr.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://amk.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://dzh.jqgfzy.top

Java: s.lines().toList()
来源：http://ozc.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://wuj.gotoacloud.top

Ruby: s.lines
来源：http://oar.ydjk.org.cn

C#:   s.Split('\n')
来源：http://gtk.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://nfb.kuanghao11.cn

Py:   if not s:
来源：http://yvb.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fxu.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://huj.aibaodan.cn

TS:   if (s === "") {}
来源：http://qqi.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://oad.nanxuanxn.top

Go:   if s == "" {}
来源：http://qis.iojbl.cn

Ruby: if s.empty?
来源：http://rmp.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ddf.svipenyu.cn

[E21] 超长截断加省略号
来源：http://xfs.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fvq.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vfv.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tfx.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfj.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fle.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://tmq.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://egp.andypj.xyz

[E22] 字节长度与字符长度
来源：http://jru.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ztl.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tjy.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://plo.jqgufenzy.top


<!-- 参考信息 -->