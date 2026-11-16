代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ebo.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gmg.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://ush.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://azx.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://htt.smart0.xyz

Go:   // 手写循环
来源：http://umu.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://upa.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zvv.jinqigfzy.top

[D15] 去重
来源：http://ubo.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ris.52xcode.cn

PHP:  array_unique($arr);
来源：http://iyz.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://tfi.52xcode.cn

TS:   [...new Set(arr)]
来源：http://cno.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://psh.tanke756.top

Go:   // 用 map[T]struct{} 手写
来源：http://dku.hysaishi.cn

Ruby: arr.uniq
来源：http://pof.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://nnx.ppjwa.cn

[D16] 求和与平均值
来源：http://kfw.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ofs.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wwc.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nkf.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://syf.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fug.cdnleiting.top

Go:   // 手写循环累加
来源：http://nyn.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fis.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://kez.zhongyouzk.top

[D17] 最大值与最小值
来源：http://uva.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://cbo.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://yaz.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xbs.ctjpmb.com

TS:   Math.max(...arr);
来源：http://ply.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://udd.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bpj.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://qjm.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://xfc.316326.xyz

[D18] 扁平化嵌套数组
来源：http://tnv.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lqj.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://gge.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bna.yj202588.top

TS:   nested.flat();
来源：http://gmq.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wtf.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://ihj.gaohongyu789.top

Ruby: nested.flatten
来源：http://fwn.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yik.gotoacloud.top

[D19] 按字段分组
来源：http://yso.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mno.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dqi.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ork.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jxr.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wev.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://vph.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uqr.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qgu.meibo888.top

[D20] 统计每个元素出现次数
来源：http://ilg.shzxlz.cn

Py:   Counter(arr)
来源：http://ppw.zhijiandao.cn

PHP:  array_count_values($arr);
来源：http://qao.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vjc.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nel.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kwc.epnwcf.com

Go:   // 手写 map[T]int
来源：http://enh.yueranfly.top

Ruby: arr.tally
来源：http://nzu.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zrw.tarul.cn

[D21] 判断是否包含某元素
来源：http://zok.hfpthk.cn

Py:   x in arr
来源：http://fkk.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://dge.yuxming.cn

JS:   arr.includes(x)
来源：http://mfi.jqgufenzy.top

TS:   arr.includes(x)
来源：http://yxq.guannengcc.top

Java: list.contains(x)
来源：http://sys.zdbjq.cn

Go:   slices.Contains(arr, x)
来源：http://btd.jqgfzy.top

Ruby: arr.include?(x)
来源：http://era.nwbrower.top

C#:   list.Contains(x)
来源：http://ovj.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://gts.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cyg.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jzj.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tiu.tian-w.cn

TS:   [...arr];
来源：http://pjm.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://jzv.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://prj.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://ngg.smart0.xyz

C#:   new List<int>(list);
来源：http://qbh.shuidangran.top

[D23] reduce 累积计算
来源：http://nvz.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vjh.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oix.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpt.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://obe.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nia.bjfxy.top

Go:   // 手写循环
来源：http://rgu.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xir.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nxb.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://rkg.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sjx.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wlf.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vzx.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sxa.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xsv.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sls.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ozo.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hlw.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://cws.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cpu.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vpz.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gfh.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fdf.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mgo.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lnq.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://niy.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iyj.birdmap.top

[D26] 数组转字符串
来源：http://twz.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://yke.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://qst.cashguo.top

JS:   arr.join(", ")
来源：http://azy.bjfxy.top

TS:   arr.join(", ")
来源：http://saq.snrcjt.cn

Java: String.join(", ", list)
来源：http://wvf.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://sly.yj20258888.top

Ruby: arr.join(", ")
来源：http://fyu.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://xqw.bjfxy.top

================================================================================
来源：http://xab.jqgfzy.top

E. 字符串处理
来源：http://rga.iojbl.cn

================================================================================
来源：http://mxb.gotoacloud.top

[E01] 拼接字符串
来源：http://vaj.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://loy.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fde.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aae.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rrf.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jes.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ckc.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bsw.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nhp.316326.xyz

[E02] 重复字符串
来源：http://zkg.redwolf501.top

Py:   "ab" * 3
来源：http://tvt.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://ayl.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://izu.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://pvr.gogol.net.cn

Java: "ab".repeat(3)
来源：http://joi.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://kbt.pycfn.com

Ruby: "ab" * 3
来源：http://bwt.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://smo.yuanzhike.top

[E03] 截取子串
来源：http://usi.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rpz.yj20258888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bki.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kuo.yj20258888.top

TS:   s.slice(1, 4)
来源：http://xzc.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://xpi.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ovn.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://zew.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://bie.tian-w.cn

[E04] 查找子串位置
来源：http://swv.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://ibk.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://nio.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://stf.zycfv.cn

TS:   s.indexOf("x")
来源：http://nct.zhoulong.xyz

Java: s.indexOf("x")
来源：http://kar.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://kkm.vehdjk.com

Ruby: s.index("x")
来源：http://vsi.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://bul.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xzr.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yth.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lgt.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kqn.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lmc.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fxi.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xyy.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eit.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lhx.hesvh.cn

[E06] 替换子串
来源：http://ofm.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iax.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://bvb.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tjj.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://lwa.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qfd.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zgd.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://loo.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://bhc.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://ksv.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hik.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://krq.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ifo.nanxuanxn.top

TS:   s.split(",")
来源：http://xgz.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kly.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bwv.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://xql.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://knp.yongpay.top

[E08] 数组按分隔符合并
来源：http://ozi.ivvv.top

Py:   ",".join(items)
来源：http://bvo.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://ypr.sweek.top

JS:   items.join(",")
来源：http://occ.hammf.cn

TS:   items.join(",")
来源：http://abg.zhijiandao.cn

Java: String.join(",", items)
来源：http://gjp.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://sdr.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://aur.yfazqb.com

C#:   string.Join(",", items)
来源：http://vrc.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://seh.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://orr.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://izo.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://tkg.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://rdu.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://yrp.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://crb.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://akg.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zxe.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://wcm.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gtx.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gvx.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://bbb.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://oiw.daxiang520.top

Java: String.format("%03d", 7)
来源：http://clg.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qqq.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vin.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ipk.nanxuanxn.top

[E11] 反转字符串
来源：http://xee.ppjwa.cn

Py:   s[::-1]
来源：http://ktb.snrcjt.cn

PHP:  strrev($s);
来源：http://akn.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://dvs.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://tfu.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://djd.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xvh.yueranfly.top

Ruby: s.reverse
来源：http://yrd.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nos.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://brl.tarul.cn

Py:   s.count("a")
来源：http://cds.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://ucg.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://ckf.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://jrr.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ynu.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://zld.meibo888.top

Ruby: s.count("a")
来源：http://iup.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://omz.gotoacloud.top

[E13] 逐字符遍历
来源：http://rxl.havefunace.top

Py:   for ch in s: print(ch)
来源：http://xlf.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vxc.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zas.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://geq.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rlk.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wke.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://bgu.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://btf.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://blz.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fyy.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cnl.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ung.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://syz.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mlq.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eet.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wnl.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qin.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://acd.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fso.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bcq.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dfs.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pyi.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://anc.daxiang520.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ynk.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ebw.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xcv.shangyingyoupin.top

[E16] 数字千分位
来源：http://zmo.bbcook.cn

Py:   f"{1234567:,}"
来源：http://ihe.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://nmm.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vif.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://uhx.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dzc.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vcc.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://phi.meibo888.top

C#:   1234567.ToString("N0")
来源：http://gyv.bjfxy.top

[E17] 首字母大写
来源：http://vrf.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://liv.0kj1m.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uvk.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tuz.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qzq.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://koa.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://psi.zdbjq.cn

Ruby: s.capitalize
来源：http://siq.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hyz.cdnleiting.top

[E18] 模板占位符替换
来源：http://ayr.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://unl.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mza.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tuw.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wsw.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://siu.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rvq.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tnr.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ign.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://jei.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://hfd.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ejk.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://dlr.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://lof.zhijiandao.cn

Java: s.lines().toList()
来源：http://zzg.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://zdh.yj20258888.top

Ruby: s.lines
来源：http://bui.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://iay.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://geh.snrcjt.cn

Py:   if not s:
来源：http://wqk.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bxx.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://unc.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://owg.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://aug.jiagoushi.top

Go:   if s == "" {}
来源：http://ywr.tanke756.top

Ruby: if s.empty?
来源：http://rcg.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://syx.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://lof.jlsjyb.cn


<!-- 参考信息 -->