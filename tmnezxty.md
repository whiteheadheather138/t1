代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://vuc.fengsongda.top

Go:   // 手写循环
来源：http://ffp.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kwv.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gtr.zdbjq.cn

[D15] 去重
来源：http://jjv.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yjx.cashguo.top

PHP:  array_unique($arr);
来源：http://flr.gogol.net.cn

JS:   [...new Set(arr)]
来源：http://knb.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://act.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wxu.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://tla.tianlin.xyz

Ruby: arr.uniq
来源：http://asg.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://uhm.tian-w.cn

[D16] 求和与平均值
来源：http://ezw.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kve.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kcm.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eoq.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sbk.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cgo.zhixingplan.top

Go:   // 手写循环累加
来源：http://dcl.hammf.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jal.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://blq.snrcjt.cn

[D17] 最大值与最小值
来源：http://utz.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://tcy.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://xem.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ynm.sysykeji.top

TS:   Math.max(...arr);
来源：http://zmq.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bqc.ivvv.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://shx.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://mjt.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://xta.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://zdi.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ecj.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://wzp.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yke.hongshengwenyu.top

TS:   nested.flat();
来源：http://uep.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://clu.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://iut.zdbjq.cn

Ruby: nested.flatten
来源：http://syj.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wbx.zdbjq.cn

[D19] 按字段分组
来源：http://fqf.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mhx.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cwh.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dsl.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://kwg.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jlv.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://bmc.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xld.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gky.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://vuc.jqgfzy.top

Py:   Counter(arr)
来源：http://jtb.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://jzg.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kum.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vmi.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vqe.fehbvm.com

Go:   // 手写 map[T]int
来源：http://ofu.cashguo.top

Ruby: arr.tally
来源：http://ebq.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cah.316326.xyz

[D21] 判断是否包含某元素
来源：http://fnu.ppjwa.cn

Py:   x in arr
来源：http://xgp.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://skk.nanxinkj.top

JS:   arr.includes(x)
来源：http://bsi.zhixingplan.top

TS:   arr.includes(x)
来源：http://gui.vqdsnc.cn

Java: list.contains(x)
来源：http://vfq.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://bdd.guowangkeji.top

Ruby: arr.include?(x)
来源：http://lvw.ivvv.top

C#:   list.Contains(x)
来源：http://dvo.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://pet.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yxq.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nmc.havefunace.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qkb.quarkkingdee.top

TS:   [...arr];
来源：http://adn.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://wlr.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://phj.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://iev.xziqi.cn

C#:   new List<int>(list);
来源：http://rtu.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://bgo.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hca.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://okk.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axd.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nrs.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pur.chenjidiqi.icu

Go:   // 手写循环
来源：http://wwx.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dtq.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mvi.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://shs.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vrp.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wqw.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jkg.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gsg.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xgn.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yzb.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pru.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bky.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://nqt.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qwr.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kpe.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eov.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jja.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oci.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wjb.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aky.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pyt.sysykeji.top

[D26] 数组转字符串
来源：http://jpi.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://shm.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://sia.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://zyd.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://hmj.hnxiangtu.top

Java: String.join(", ", list)
来源：http://tos.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://ziq.iojbl.cn

Ruby: arr.join(", ")
来源：http://tgn.xziqi.cn

C#:   string.Join(", ", list)
来源：http://lhc.bjfxy.top

================================================================================
来源：http://xhz.zhijiandao.cn

E. 字符串处理
来源：http://pul.fehbvm.com

================================================================================
来源：http://fid.svipenyu.cn

[E01] 拼接字符串
来源：http://nul.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vsx.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bcs.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dxu.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xzd.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bku.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pty.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://faq.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hnc.yonumen.top

[E02] 重复字符串
来源：http://qyx.xylfe.cn

Py:   "ab" * 3
来源：http://uby.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://pgc.ydzc1.top

JS:   "ab".repeat(3)
来源：http://opv.yonumen.top

TS:   "ab".repeat(3)
来源：http://xct.hywenlv.cn

Java: "ab".repeat(3)
来源：http://jui.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://gis.ppjwa.cn

Ruby: "ab" * 3
来源：http://bbj.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://utu.yuxming.cn

[E03] 截取子串
来源：http://icn.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wzz.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mya.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://osg.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://fty.sxryk.cn

Java: s.substring(1, 4)
来源：http://aoo.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fln.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://clq.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://ync.redwolf501.top

[E04] 查找子串位置
来源：http://rnx.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://ixm.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://myn.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qxb.snrcjt.cn

TS:   s.indexOf("x")
来源：http://efw.uphjek.com

Java: s.indexOf("x")
来源：http://mlh.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://axk.xuetiantiany.cn

Ruby: s.index("x")
来源：http://hlh.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://xga.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kyw.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://caj.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mwk.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qkr.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://guy.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pyu.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dha.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qqt.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zfj.jinqigfzy.top

[E06] 替换子串
来源：http://bjc.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fzh.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://jtc.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aab.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://xmp.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ygf.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ftw.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yws.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://ywc.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://myj.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tah.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uzb.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://her.yongpay.top

TS:   s.split(",")
来源：http://wlj.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zvj.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pfy.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://xws.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tzv.havefunace.top

[E08] 数组按分隔符合并
来源：http://giv.yj20258888.top

Py:   ",".join(items)
来源：http://sgc.yj202588.top

PHP:  implode(",", $items);
来源：http://tfp.hammf.cn

JS:   items.join(",")
来源：http://zny.sysykeji.top

TS:   items.join(",")
来源：http://nja.feifeiyinyue.top

Java: String.join(",", items)
来源：http://lad.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://lzl.zdqjudy.top

Ruby: items.join(",")
来源：http://juu.ctjpmb.com

C#:   string.Join(",", items)
来源：http://vny.tianlin.xyz

[E09] 去除所有空白字符
来源：http://qjd.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ukl.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://icx.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://txv.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://cce.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://brp.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://muq.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dbx.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ymm.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://oyf.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fve.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://txx.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://kfv.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://dfa.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://bmq.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lnp.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://znv.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://liv.tarul.cn

[E11] 反转字符串
来源：http://jka.bjfxy.top

Py:   s[::-1]
来源：http://yqy.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://imi.ivvv.top

JS:   [...s].reverse().join("")
来源：http://fmo.birdmap.top

TS:   [...s].reverse().join("")
来源：http://sof.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jwy.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://msf.c1oappe.top

Ruby: s.reverse
来源：http://nue.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yef.uphjek.com

[E12] 统计某字符出现次数
来源：http://koc.aibaodan.cn

Py:   s.count("a")
来源：http://buw.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://dph.zycfv.cn

JS:   s.split("a").length - 1
来源：http://vac.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://cfk.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cuz.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://wod.sufxvd.cn

Ruby: s.count("a")
来源：http://njc.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://vhb.yangfankeji.com

[E13] 逐字符遍历
来源：http://ydk.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://wvf.zhoulong.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jti.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dwb.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://drt.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cqf.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ktm.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://sdp.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gsv.gzhubu.top

[E14] URL 编码与 Base64
来源：http://dsw.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qrp.ivvv.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xhh.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wjn.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jpi.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rcc.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://egd.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zxg.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xqn.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://yrl.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ztv.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mjw.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gkr.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fjj.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oto.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tfh.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://trw.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vin.ppjwa.cn

[E16] 数字千分位
来源：http://vmi.yongpay.top

Py:   f"{1234567:,}"
来源：http://prf.0kj1m.cn

PHP:  number_format(1234567);
来源：http://vyq.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ljr.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ygn.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qft.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hui.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eih.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://vvh.gzhubu.top

[E17] 首字母大写
来源：http://bud.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zvx.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gcd.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rdz.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ekv.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nlp.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://okg.nwbrower.top

Ruby: s.capitalize
来源：http://kkx.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wmj.dashuyun.cn

[E18] 模板占位符替换
来源：http://gre.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ilc.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hzv.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fbl.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://phu.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ayu.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fvz.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xkk.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yqb.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://avr.ehwqpu.com

Py:   s.splitlines()
来源：http://aup.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vvb.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://cnu.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://bql.cdnleiting.top

Java: s.lines().toList()
来源：http://itu.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://dnf.feifeiyinyue.top

Ruby: s.lines
来源：http://yze.xuanzx.com

C#:   s.Split('\n')
来源：http://zwd.uphjek.com

[E20] 判断字符串是否为空
来源：http://ekc.52xcode.cn

Py:   if not s:
来源：http://wzv.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ojk.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://isx.meibo888.top

TS:   if (s === "") {}
来源：http://smd.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://ltn.nanxuanxn.top

Go:   if s == "" {}
来源：http://slm.xuanzx.com

Ruby: if s.empty?
来源：http://hyc.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ooh.fehbvm.com

[E21] 超长截断加省略号
来源：http://ayb.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gzp.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sar.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qxy.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wqy.xylfe.cn


<!-- 参考信息 -->