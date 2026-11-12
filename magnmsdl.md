代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://slc.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jti.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://puf.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://tpt.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lzk.cheryme.top

Go:   // 手写循环
来源：http://jbk.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://plo.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xib.nanxinkj.top

[D15] 去重
来源：http://umt.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://foq.meibo888.top

PHP:  array_unique($arr);
来源：http://kwr.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://kge.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://tlq.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nbh.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://szn.kuanghao11.cn

Ruby: arr.uniq
来源：http://byv.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://vmh.iojbl.cn

[D16] 求和与平均值
来源：http://yqh.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gsm.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eyz.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kba.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yjk.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jkg.tianlin.xyz

Go:   // 手写循环累加
来源：http://cjk.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nsa.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://wpu.zdqjudy.top

[D17] 最大值与最小值
来源：http://mhu.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://sdt.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://yea.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dxe.yuanzhike.top

TS:   Math.max(...arr);
来源：http://qve.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gxz.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vdi.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://qid.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://tvq.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://ibo.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://czf.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://gvh.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sxk.shanyushiyangtech.top

TS:   nested.flat();
来源：http://rij.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rot.c1oappe.top

Go:   // 手写双层循环
来源：http://ezb.c1oappe.top

Ruby: nested.flatten
来源：http://ejf.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iuf.wangshuangyany.cn

[D19] 按字段分组
来源：http://mge.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ixh.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tmn.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gff.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://oum.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xpw.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://ngg.jqgufenzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ujk.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wmu.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://ebs.daxiang520.top

Py:   Counter(arr)
来源：http://jhe.yonumen.top

PHP:  array_count_values($arr);
来源：http://wad.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qan.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zip.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ueg.hesvh.cn

Go:   // 手写 map[T]int
来源：http://bzn.iojbl.cn

Ruby: arr.tally
来源：http://jpf.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://izo.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://xuc.xuetiantiany.cn

Py:   x in arr
来源：http://fxl.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://brq.sweek.top

JS:   arr.includes(x)
来源：http://uls.nwbrower.top

TS:   arr.includes(x)
来源：http://jkd.xinyue.icu

Java: list.contains(x)
来源：http://vkj.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://bxs.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://ris.yuanzhike.top

C#:   list.Contains(x)
来源：http://tgh.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://ssf.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mpo.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qvt.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bwb.shuidangran.top

TS:   [...arr];
来源：http://ftc.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://der.yongpay.top

Go:   copied := append([]int(nil), arr...)
来源：http://gsy.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://rpr.zhoulong.xyz

C#:   new List<int>(list);
来源：http://gwo.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://sem.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aqb.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rtv.havefunace.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://asb.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dct.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nvn.daxiang520.top

Go:   // 手写循环
来源：http://nzl.bbcook.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hpt.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nam.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://ngx.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dbx.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jhm.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ntd.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eax.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://llp.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lkz.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://udi.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lrr.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://rqm.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rgy.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jsz.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ssg.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iwh.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tym.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hcw.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jet.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bmi.cucudq.cn

[D26] 数组转字符串
来源：http://eam.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://mnt.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://bfk.vehdjk.com

JS:   arr.join(", ")
来源：http://rzw.nanxuanxn.top

TS:   arr.join(", ")
来源：http://qjn.316326.xyz

Java: String.join(", ", list)
来源：http://dwv.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://qce.yongpay.top

Ruby: arr.join(", ")
来源：http://bum.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://epv.jlsjyb.cn

================================================================================
来源：http://qqo.hnqzz.top

E. 字符串处理
来源：http://hlt.316326.xyz

================================================================================
来源：http://ffj.fzhhl.top

[E01] 拼接字符串
来源：http://qig.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ilp.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bxp.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yoo.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jad.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zew.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mdp.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oqs.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gdp.sysykeji.top

[E02] 重复字符串
来源：http://iqd.kuanghao11.cn

Py:   "ab" * 3
来源：http://soj.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://cdb.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://lsn.wangdashe.top

TS:   "ab".repeat(3)
来源：http://boo.chenzaomai.com

Java: "ab".repeat(3)
来源：http://kqc.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://mtf.cqqwz.cn

Ruby: "ab" * 3
来源：http://iqr.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dgf.xziqi.cn

[E03] 截取子串
来源：http://gsq.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://siu.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nuy.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xkv.ybcxt.top

TS:   s.slice(1, 4)
来源：http://dyy.shuidangran.top

Java: s.substring(1, 4)
来源：http://vzj.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ehq.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ohf.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://pgs.gaohongyu789.top

[E04] 查找子串位置
来源：http://coz.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://ugb.shuidangran.top

PHP:  strpos($s, "x");
来源：http://bav.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gfh.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://pxp.jlsjyb.cn

Java: s.indexOf("x")
来源：http://mfz.yonumen.top

Go:   strings.Index(s, "x")
来源：http://psv.hesvh.cn

Ruby: s.index("x")
来源：http://ihx.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://yoq.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://iwk.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fck.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pxe.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://prj.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oai.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://byl.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xfo.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jzq.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mtd.jyoumei.cn

[E06] 替换子串
来源：http://icv.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vlk.smart0.xyz

PHP:  str_replace("a", "b", $s);
来源：http://jxe.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ual.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://xgl.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ixv.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yui.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lkd.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://cfy.pycfn.com

[E07] 按分隔符拆分
来源：http://uog.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xlg.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jtn.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lag.yongpay.top

TS:   s.split(",")
来源：http://amb.yfazqb.com

Java: s.split(",");  s.split("\\s+")
来源：http://vys.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nej.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://ego.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oav.yj20258888.top

[E08] 数组按分隔符合并
来源：http://lxb.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://ebp.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://gty.daxiang520.top

JS:   items.join(",")
来源：http://jdf.zycfv.cn

TS:   items.join(",")
来源：http://rgj.hesvh.cn

Java: String.join(",", items)
来源：http://lyi.sweek.top

Go:   strings.Join(items, ",")
来源：http://dyc.cashguo.top

Ruby: items.join(",")
来源：http://stv.zhengqikj.top

C#:   string.Join(",", items)
来源：http://fmn.jianghu66.top

[E09] 去除所有空白字符
来源：http://lpw.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mvl.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ojm.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://lhn.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://uwc.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://hhb.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://rmz.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://qwi.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gki.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://msw.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ydl.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fmi.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://lki.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://lzg.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://zen.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://taa.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://azr.tianlin.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sbl.zdbjq.cn

[E11] 反转字符串
来源：http://cwx.xylfe.cn

Py:   s[::-1]
来源：http://dvn.cucudq.cn

PHP:  strrev($s);
来源：http://akj.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://ubu.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://mky.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://omi.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://axx.guannengcc.top

Ruby: s.reverse
来源：http://ihn.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://rbn.hnqzz.top

[E12] 统计某字符出现次数
来源：http://tiz.yonumen.top

Py:   s.count("a")
来源：http://pzw.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://lry.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://cor.havefunace.top

TS:   s.split("a").length - 1
来源：http://xev.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ofl.ywan-chungtsiang.top

Go:   strings.Count(s, "a")
来源：http://ibj.svipenyu.cn

Ruby: s.count("a")
来源：http://ipl.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://cui.sxryk.cn

[E13] 逐字符遍历
来源：http://vvl.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://rjm.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bfo.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lga.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ybu.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jjg.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mtf.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://oci.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uwh.yonumen.top

[E14] URL 编码与 Base64
来源：http://bcu.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eaz.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bjb.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qxl.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mqq.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yca.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ups.iojbl.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qcc.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wls.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://jkv.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xpb.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hsi.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qtr.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://qfx.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://osl.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mts.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fap.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tye.316326.xyz

[E16] 数字千分位
来源：http://dec.yj202588.top

Py:   f"{1234567:,}"
来源：http://qba.jianghu66.top

PHP:  number_format(1234567);
来源：http://ige.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dox.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xwi.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rao.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nbi.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cbd.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://nlj.xinyue.icu

[E17] 首字母大写
来源：http://vkd.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://phu.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mcx.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kuc.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mec.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qqp.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yst.hysaishi.cn

Ruby: s.capitalize
来源：http://yko.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://chf.cdnleiting.top

[E18] 模板占位符替换
来源：http://mid.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://toi.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://omq.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://czu.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://exy.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gly.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://igh.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cwz.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bxy.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://vfk.aizwys.cn

Py:   s.splitlines()
来源：http://ksl.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://toa.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://wfh.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://sqr.hesvh.cn

Java: s.lines().toList()
来源：http://iqj.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://dsf.nwbrower.top

Ruby: s.lines
来源：http://jbh.yj20258888.top

C#:   s.Split('\n')
来源：http://epu.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://urp.pengpengdd.cyou

Py:   if not s:
来源：http://npy.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zar.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wpd.aibaodan.cn

TS:   if (s === "") {}
来源：http://ejc.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://uwb.yanxiufei.cn

Go:   if s == "" {}
来源：http://rjw.vqdsnc.cn

Ruby: if s.empty?
来源：http://qac.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fvl.shzxlz.cn

[E21] 超长截断加省略号
来源：http://jpk.yfazqb.com


<!-- 参考信息 -->