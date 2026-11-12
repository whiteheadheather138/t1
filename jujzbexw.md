代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://xee.jqgufenzy.top

Go:   // 手写循环
来源：http://fch.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://chr.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gtd.ctjpmb.com

[D15] 去重
来源：http://tmy.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pqd.gzhubu.top

PHP:  array_unique($arr);
来源：http://cxb.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://izh.yueranfly.top

TS:   [...new Set(arr)]
来源：http://dxq.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rmz.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://ead.tarul.cn

Ruby: arr.uniq
来源：http://uul.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://rbp.ppjwa.cn

[D16] 求和与平均值
来源：http://ifx.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uio.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dsz.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mny.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgj.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wyx.meibo888.top

Go:   // 手写循环累加
来源：http://skw.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gjo.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://oax.tian-w.cn

[D17] 最大值与最小值
来源：http://kem.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://zfx.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://tkk.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blb.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://giz.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vxy.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aan.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://iov.yonumen.top

C#:   list.Max();  list.Min()
来源：http://nja.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://qji.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sib.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://nmv.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fyh.gzhubu.top

TS:   nested.flat();
来源：http://yer.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tcu.hywenlv.cn

Go:   // 手写双层循环
来源：http://pjb.yanxiufei.cn

Ruby: nested.flatten
来源：http://aok.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ecs.hammf.cn

[D19] 按字段分组
来源：http://lec.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gkq.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jjs.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kpk.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uwj.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ogj.pycfn.com

Go:   // 手写 map[string][]T
来源：http://xmx.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nao.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hoz.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://bnx.sysykeji.top

Py:   Counter(arr)
来源：http://uxk.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://xge.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ofr.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kld.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://etl.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://ijr.wangshuangyany.cn

Ruby: arr.tally
来源：http://ejo.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jlh.xziqi.cn

[D21] 判断是否包含某元素
来源：http://jli.gotoacloud.top

Py:   x in arr
来源：http://lpe.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://zgi.0kj1m.cn

JS:   arr.includes(x)
来源：http://yzr.ydjk.org.cn

TS:   arr.includes(x)
来源：http://ubz.9152youxi.cn

Java: list.contains(x)
来源：http://snn.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://ukw.yuanzhike.top

Ruby: arr.include?(x)
来源：http://cgn.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://qwt.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://asm.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://llq.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pmk.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lqt.c1oappe.top

TS:   [...arr];
来源：http://wmh.ybcxt.top

Java: new ArrayList<>(list);
来源：http://ytv.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://lsl.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://cvs.gaohongyu789.top

C#:   new List<int>(list);
来源：http://err.ydjk.org.cn

[D23] reduce 累积计算
来源：http://skb.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tqi.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://esz.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://opb.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zhs.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jos.shzxlz.cn

Go:   // 手写循环
来源：http://bly.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kvl.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ces.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://uzc.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tbl.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tje.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ttj.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://win.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://evv.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vsc.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://akn.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tgz.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://ysv.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://egd.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jji.fehbvm.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mgm.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bmi.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://whu.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lrj.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bic.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pjr.xylfe.cn

[D26] 数组转字符串
来源：http://vof.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://ypf.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://xgg.9152youxi.cn

JS:   arr.join(", ")
来源：http://yms.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://vpo.cdnleiting.top

Java: String.join(", ", list)
来源：http://jae.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://lzk.nanxinkj.top

Ruby: arr.join(", ")
来源：http://btf.guannengcc.top

C#:   string.Join(", ", list)
来源：http://cjn.zdbjq.cn

================================================================================
来源：http://pwu.yonumen.top

E. 字符串处理
来源：http://dyc.dashuyun.cn

================================================================================
来源：http://jjf.chenjidiqi.icu

[E01] 拼接字符串
来源：http://jvs.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vdr.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ysu.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://unk.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dax.dianchejie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xmv.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fix.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://stb.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ayt.uphjek.com

[E02] 重复字符串
来源：http://lhd.kuanghao11.cn

Py:   "ab" * 3
来源：http://ydi.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://azt.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://swu.hcnkem.com

TS:   "ab".repeat(3)
来源：http://cfr.9152youxi.cn

Java: "ab".repeat(3)
来源：http://wgy.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://syw.epnwcf.com

Ruby: "ab" * 3
来源：http://uah.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vjn.zhengqikj.top

[E03] 截取子串
来源：http://vyp.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lgf.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kfj.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fay.jyoumei.cn

TS:   s.slice(1, 4)
来源：http://eyb.zdqjudy.top

Java: s.substring(1, 4)
来源：http://tty.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://epv.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://ony.316326.xyz

C#:   s.Substring(1, 3)
来源：http://lxg.dianchejie.cn

[E04] 查找子串位置
来源：http://wib.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://pbr.c1oappe.top

PHP:  strpos($s, "x");
来源：http://zuq.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mdh.fengsongda.top

TS:   s.indexOf("x")
来源：http://yec.kuanghao11.cn

Java: s.indexOf("x")
来源：http://twx.ehwqpu.com

Go:   strings.Index(s, "x")
来源：http://xdv.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://nqb.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://wxt.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cpb.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nri.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://spo.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dqr.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bwy.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://siu.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uyc.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vbn.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://onl.dianchejie.cn

[E06] 替换子串
来源：http://gxw.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xpc.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://tdc.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://crj.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://oyx.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://snu.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lyt.shanyushiyangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dti.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://ipq.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://fyy.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ivs.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bef.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://nxh.hnqzz.top

TS:   s.split(",")
来源：http://dzz.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://nvm.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iwo.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://jwx.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vrd.fzhhl.top

[E08] 数组按分隔符合并
来源：http://pfy.yuanzhike.top

Py:   ",".join(items)
来源：http://cuo.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://bda.shanyushiyangtech.top

JS:   items.join(",")
来源：http://xbs.vehdjk.com

TS:   items.join(",")
来源：http://ukn.vehdjk.com

Java: String.join(",", items)
来源：http://kco.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://vpr.gotoacloud.top

Ruby: items.join(",")
来源：http://iqy.jiagoushi.top

C#:   string.Join(",", items)
来源：http://uvb.jyoumei.cn

[E09] 去除所有空白字符
来源：http://ioz.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://alt.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dab.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://svd.yj202588.top

TS:   s.replace(/\s+/g, "")
来源：http://qim.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xfs.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dsv.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wvx.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ufw.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://zvn.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hre.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ytw.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://qie.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://rwk.yuxming.cn

Java: String.format("%03d", 7)
来源：http://bga.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hqj.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mqz.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yuq.uphjek.com

[E11] 反转字符串
来源：http://cxx.zycfv.cn

Py:   s[::-1]
来源：http://wqe.nanxuanxn.top

PHP:  strrev($s);
来源：http://rzs.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://imu.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://iot.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zok.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qak.hnqzz.top

Ruby: s.reverse
来源：http://yrr.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://dct.shangyingyoupin.top

[E12] 统计某字符出现次数
来源：http://ror.gogol.net.cn

Py:   s.count("a")
来源：http://ucr.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://ogq.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://odv.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://erf.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ruq.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://wub.hnqzz.top

Ruby: s.count("a")
来源：http://yfy.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://zue.epnwcf.com

[E13] 逐字符遍历
来源：http://buf.cashguo.top

Py:   for ch in s: print(ch)
来源：http://eul.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xwf.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wqx.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://swk.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ukc.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qha.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sxx.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xkg.hnqzz.top

[E14] URL 编码与 Base64
来源：http://vfw.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xyh.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bem.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://joe.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vtz.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ajb.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pdp.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dtx.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://day.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://dmr.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://djc.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yoc.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hqx.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ika.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://syr.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://frc.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cca.jiagoushi.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sck.jianghu66.top

[E16] 数字千分位
来源：http://yhu.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://hro.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://rsw.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ywr.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hsg.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uro.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iwd.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tcs.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://hhi.cucudq.cn

[E17] 首字母大写
来源：http://rep.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eet.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vqh.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cpk.ehwqpu.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uzi.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sgf.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hhu.hfpthk.cn

Ruby: s.capitalize
来源：http://pdt.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://slg.yuxming.cn

[E18] 模板占位符替换
来源：http://bwi.316326.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://prj.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vko.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jyr.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mwm.yueranfly.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://crf.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ulv.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qqf.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cqt.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://wbe.tianlin.xyz

Py:   s.splitlines()
来源：http://ozh.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ker.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://jmo.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://czq.0kj1m.cn

Java: s.lines().toList()
来源：http://xmk.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://xil.cucudq.cn

Ruby: s.lines
来源：http://wev.ydzc1.top

C#:   s.Split('\n')
来源：http://iyo.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://viy.mhx1999.top

Py:   if not s:
来源：http://hmq.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yqo.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ziz.kuanghao11.cn

TS:   if (s === "") {}
来源：http://xoy.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://off.jinqigufen.top

Go:   if s == "" {}
来源：http://fyb.yj202588.top

Ruby: if s.empty?
来源：http://jvx.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://edu.dashuyun.cn

[E21] 超长截断加省略号
来源：http://yry.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sym.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mzh.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zny.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://msn.cdnleiting.top


<!-- 参考信息 -->