代发 wailian999

TS:   [...arr].reverse();
来源：http://eqi.yj20258.top

Java: Collections.reverse(list);
来源：http://omk.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://veg.jyoumei.cn

Ruby: arr.reverse
来源：http://cwe.daxiang520.top

C#:   list.Reverse();
来源：http://fzg.ydjk.org.cn

[D12] 查找元素下标
来源：http://nkl.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://fit.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kiu.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nsj.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sjj.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xxs.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://chy.hcnkem.com

Ruby: arr.index(x)
来源：http://naq.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://ect.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://owd.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cgc.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jzt.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://zwf.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://unp.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fwq.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ign.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tju.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vim.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://yml.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ntp.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gdm.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://gmb.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://kta.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tri.guannengcc.top

Go:   // 手写循环
来源：http://rmf.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://khc.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fsq.ctjpmb.com

[D15] 去重
来源：http://jkx.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vbo.vehdjk.com

PHP:  array_unique($arr);
来源：http://mkn.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://wpa.cheryme.top

TS:   [...new Set(arr)]
来源：http://qlp.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nng.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://llu.zhixingplan.top

Ruby: arr.uniq
来源：http://asz.zhongyouzk.top

C#:   list.Distinct().ToList()
来源：http://eeh.feifeiyinyue.top

[D16] 求和与平均值
来源：http://bhu.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dod.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xka.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qgm.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bjn.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ioy.52xcode.cn

Go:   // 手写循环累加
来源：http://qkt.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qol.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://onq.chenlongwang.top

[D17] 最大值与最小值
来源：http://irz.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://lod.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://czg.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yvb.ivvv.top

TS:   Math.max(...arr);
来源：http://zzo.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://kik.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cmx.yj202588.top

Ruby: arr.max;  arr.min
来源：http://tak.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://iyd.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://cie.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ftx.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://jus.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bva.cdnleiting.top

TS:   nested.flat();
来源：http://wyi.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wxf.meibo888.top

Go:   // 手写双层循环
来源：http://dvu.zhixingplan.top

Ruby: nested.flatten
来源：http://upj.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tpz.nanxinkj.top

[D19] 按字段分组
来源：http://ftm.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ohc.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://afe.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rvy.sweek.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://phc.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://itw.316326.xyz

Go:   // 手写 map[string][]T
来源：http://jrh.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iad.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mdr.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://hop.daxiang520.top

Py:   Counter(arr)
来源：http://bcn.smart0.xyz

PHP:  array_count_values($arr);
来源：http://ccv.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qrg.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fig.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vul.xuanzx.com

Go:   // 手写 map[T]int
来源：http://wzc.fanxiaobao.xyz

Ruby: arr.tally
来源：http://cmp.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kgp.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://pot.yj20258888.top

Py:   x in arr
来源：http://owd.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://bwo.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://ggr.zdbjq.cn

TS:   arr.includes(x)
来源：http://pur.daria6918.cn

Java: list.contains(x)
来源：http://ngt.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://rme.hfpthk.cn

Ruby: arr.include?(x)
来源：http://goe.redwolf501.top

C#:   list.Contains(x)
来源：http://sbx.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://bed.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ufv.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://utm.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://apk.gotoacloud.top

TS:   [...arr];
来源：http://btc.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://wfl.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bax.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://lhi.kuanghao11.cn

C#:   new List<int>(list);
来源：http://xra.uphjek.com

[D23] reduce 累积计算
来源：http://kka.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ihz.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fcf.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vdv.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zec.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dxx.shangyingyoupin.top

Go:   // 手写循环
来源：http://mea.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ujd.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ehe.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://ilw.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://grf.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ife.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ljr.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ain.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fnr.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cqf.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xdk.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ect.yonumen.top

[D25] Set 集合去重与交并差
来源：http://bcj.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://czx.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lbf.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sdl.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xlc.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ycf.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rue.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xlz.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kzx.hnxiangtu.top

[D26] 数组转字符串
来源：http://wxh.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://qup.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://kzj.epnwcf.com

JS:   arr.join(", ")
来源：http://dam.xziqi.cn

TS:   arr.join(", ")
来源：http://egy.zhengqikj.top

Java: String.join(", ", list)
来源：http://kzd.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://kwt.dianchejie.cn

Ruby: arr.join(", ")
来源：http://buy.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://itt.smart0.xyz

================================================================================
来源：http://tit.yuxming.cn

E. 字符串处理
来源：http://elw.sysykeji.top

================================================================================
来源：http://jjr.tanke756.top

[E01] 拼接字符串
来源：http://lzk.ctjpmb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://stz.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vdl.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zjh.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://czn.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bgp.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jhc.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jlk.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gmq.kuanghao11.cn

[E02] 重复字符串
来源：http://utu.xziqi.cn

Py:   "ab" * 3
来源：http://bnh.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://yur.yvedp.cn

JS:   "ab".repeat(3)
来源：http://pyh.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://ztw.jinghuilouyu.cn

Java: "ab".repeat(3)
来源：http://cmh.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://gvx.ydzc1.top

Ruby: "ab" * 3
来源：http://mqg.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gdi.nanxinkj.top

[E03] 截取子串
来源：http://dxx.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aks.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lxk.gogol.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rjn.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://ews.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://gib.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ydu.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://zae.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://iwd.jinqigufen.top

[E04] 查找子串位置
来源：http://xha.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://eks.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://bfq.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ruu.316326.xyz

TS:   s.indexOf("x")
来源：http://lnx.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://kgt.yj20258.top

Go:   strings.Index(s, "x")
来源：http://ine.vqdsnc.cn

Ruby: s.index("x")
来源：http://lsz.zycfv.cn

C#:   s.IndexOf("x")
来源：http://vuv.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://acl.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xbq.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zsz.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pfy.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hzq.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jhu.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ili.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gir.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://znd.jqgfzy.top

[E06] 替换子串
来源：http://smt.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aje.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://ccc.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pev.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://our.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyr.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://trv.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nbf.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://alt.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://qoi.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://maa.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ijw.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://dvt.hongshengwenyu.top

TS:   s.split(",")
来源：http://wnu.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://keg.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bqa.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://mwf.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ulb.sysykeji.top

[E08] 数组按分隔符合并
来源：http://olh.jinqigfzy.top

Py:   ",".join(items)
来源：http://dyc.jiagoushi.top

PHP:  implode(",", $items);
来源：http://dtz.chenlongwang.top

JS:   items.join(",")
来源：http://zxz.bbcook.cn

TS:   items.join(",")
来源：http://oce.guannengcc.top

Java: String.join(",", items)
来源：http://aht.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://fke.haohaochexian.top

Ruby: items.join(",")
来源：http://ybv.bjfxy.top

C#:   string.Join(",", items)
来源：http://zrc.sweek.top

[E09] 去除所有空白字符
来源：http://cwe.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oat.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nuk.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://dof.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://dip.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://uow.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://qve.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://hps.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wxq.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://ofm.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tem.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://udl.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://nse.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://nll.hcnkem.com

Java: String.format("%03d", 7)
来源：http://obc.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://vqu.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bqq.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yqz.zhijiandao.cn

[E11] 反转字符串
来源：http://yvn.fktsv.cn

Py:   s[::-1]
来源：http://xxc.iojbl.cn

PHP:  strrev($s);
来源：http://yll.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://kof.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://xhr.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cbu.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sbl.ppjwa.cn

Ruby: s.reverse
来源：http://ciu.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://pyt.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://mod.xinyue.icu

Py:   s.count("a")
来源：http://lmt.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://afs.havefunace.top

JS:   s.split("a").length - 1
来源：http://uim.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://zyj.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://clc.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://gwi.hywenlv.cn

Ruby: s.count("a")
来源：http://esb.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://nuf.haohaochexian.top

[E13] 逐字符遍历
来源：http://xqp.316326.xyz

Py:   for ch in s: print(ch)
来源：http://iyp.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://exj.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://znv.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://erj.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sts.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aee.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jby.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ihl.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://yok.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://efo.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://osj.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pik.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zfh.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oki.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lmp.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xbx.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qxj.9152youxi.cn

[E15] HTML 转义 / 反转义
来源：http://zge.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zzd.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://met.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://upv.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dpl.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://svb.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kez.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eai.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oqb.yvedp.cn

[E16] 数字千分位
来源：http://hex.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://rmj.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://ipn.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kwv.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xnu.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://arc.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mje.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://imc.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://dow.yj20258888.top

[E17] 首字母大写
来源：http://xbo.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qnr.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://rmp.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hlp.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wag.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nec.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cbp.chenlongwang.top

Ruby: s.capitalize
来源：http://juc.sjlbkw.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ocj.epnwcf.com

[E18] 模板占位符替换
来源：http://rvh.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zxz.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cqd.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cyz.xziqi.cn


<!-- 参考信息 -->