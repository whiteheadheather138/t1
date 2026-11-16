代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://naw.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wns.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://rua.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://pqj.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ftv.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yxw.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://snv.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://cce.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rtg.daria6918.cn

Go:   // 手写循环
来源：http://ulx.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://vbc.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tut.sufxvd.cn

[D15] 去重
来源：http://dgk.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://onu.mhx1999.top

PHP:  array_unique($arr);
来源：http://rni.yonumen.top

JS:   [...new Set(arr)]
来源：http://nzp.yuxming.cn

TS:   [...new Set(arr)]
来源：http://zcd.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wmr.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nav.jiagoushi.top

Ruby: arr.uniq
来源：http://pap.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://mdk.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://squ.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qru.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mqf.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmy.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yqb.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://njf.hfpthk.cn

Go:   // 手写循环累加
来源：http://aqm.smart0.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ams.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://qjo.yj20258888.top

[D17] 最大值与最小值
来源：http://kqu.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://btd.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://uoa.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oca.redwolf501.top

TS:   Math.max(...arr);
来源：http://adm.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://xuh.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ieh.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://iqb.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://hfw.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://dzn.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://omp.havefunace.top

PHP:  array_merge(...$nested);
来源：http://ftw.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uxo.guowangkeji.top

TS:   nested.flat();
来源：http://qyx.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ihc.aibaodan.cn

Go:   // 手写双层循环
来源：http://scs.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://qlk.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://aha.jlsjyb.cn

[D19] 按字段分组
来源：http://bhx.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ibc.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hxc.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://stm.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mde.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lod.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://xjs.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://glz.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://glj.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://spe.sufxvd.cn

Py:   Counter(arr)
来源：http://hqk.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://fzw.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nyy.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfu.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://epo.cqqwz.cn

Go:   // 手写 map[T]int
来源：http://pjg.cucudq.cn

Ruby: arr.tally
来源：http://olo.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dci.jianghu66.top

[D21] 判断是否包含某元素
来源：http://gfa.nanxuanxn.top

Py:   x in arr
来源：http://mlx.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://jvh.xylfe.cn

JS:   arr.includes(x)
来源：http://jum.vehdjk.com

TS:   arr.includes(x)
来源：http://kne.hongshengwenyu.top

Java: list.contains(x)
来源：http://tvb.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://sdz.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://jss.zhixingplan.top

C#:   list.Contains(x)
来源：http://tyq.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://kef.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xyy.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qdu.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mjl.gzhubu.top

TS:   [...arr];
来源：http://vqc.havefunace.top

Java: new ArrayList<>(list);
来源：http://dlz.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://tjz.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://gmj.aizwys.cn

C#:   new List<int>(list);
来源：http://cob.fehbvm.com

[D23] reduce 累积计算
来源：http://fux.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://itf.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rfb.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bmi.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byj.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hhj.wangdashe.top

Go:   // 手写循环
来源：http://glu.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aid.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wav.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://hge.zdqjudy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zay.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tic.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://orw.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hzs.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wcw.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sze.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gra.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xjf.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://glc.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ydl.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zcj.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://svq.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://axo.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lbq.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ezs.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nus.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fvq.sufxvd.cn

[D26] 数组转字符串
来源：http://ugm.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://maw.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://vqn.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://lzr.mhx1999.top

TS:   arr.join(", ")
来源：http://pbu.daria6918.cn

Java: String.join(", ", list)
来源：http://xka.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://ylu.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://gvt.bjfxy.top

C#:   string.Join(", ", list)
来源：http://rag.sufxvd.cn

================================================================================
来源：http://fct.daria6918.cn

E. 字符串处理
来源：http://muj.shanyushiyangkeji.top

================================================================================
来源：http://hsl.jyoumei.cn

[E01] 拼接字符串
来源：http://xgh.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vqd.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://epd.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xnb.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://erx.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mal.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wfl.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lzw.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cnc.hnxiangtu.top

[E02] 重复字符串
来源：http://afc.xuetiantiany.cn

Py:   "ab" * 3
来源：http://ioa.jinghuilouyu.cn

PHP:  str_repeat("ab", 3);
来源：http://izh.sysykeji.top

JS:   "ab".repeat(3)
来源：http://vuf.fzhhl.top

TS:   "ab".repeat(3)
来源：http://fuk.birdmap.top

Java: "ab".repeat(3)
来源：http://imy.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ojv.hysaishi.cn

Ruby: "ab" * 3
来源：http://gih.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://khn.ybcxt.top

[E03] 截取子串
来源：http://mzd.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ncj.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://frp.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ipk.sysykeji.top

TS:   s.slice(1, 4)
来源：http://mgy.cheryme.top

Java: s.substring(1, 4)
来源：http://luf.smart0.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ssi.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://mad.uphjek.com

C#:   s.Substring(1, 3)
来源：http://lsa.pengpengdd.cyou

[E04] 查找子串位置
来源：http://dst.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://nvz.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://opb.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://saa.yj202588.top

TS:   s.indexOf("x")
来源：http://frd.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://xhd.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://cqs.yangfankeji.com

Ruby: s.index("x")
来源：http://ogq.daria6918.cn

C#:   s.IndexOf("x")
来源：http://gag.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tmn.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dnd.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://osw.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uzs.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yzd.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sem.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vpg.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jsk.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wph.ywan-chungtsiang.top

[E06] 替换子串
来源：http://pfb.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gvc.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://dgl.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://chu.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://bvf.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jnu.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mpo.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mtq.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://tsb.yuxming.cn

[E07] 按分隔符拆分
来源：http://neu.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rul.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://avn.shangyingyoupin.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mzn.fktsv.cn

TS:   s.split(",")
来源：http://ztl.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://xzh.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gfu.yj20258888.top

Ruby: s.split(",");  s.split
来源：http://ebt.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://utg.shuidangran.top

[E08] 数组按分隔符合并
来源：http://nsp.yuxming.cn

Py:   ",".join(items)
来源：http://lan.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://pgm.meibo888.top

JS:   items.join(",")
来源：http://kcv.jinqigfzy.top

TS:   items.join(",")
来源：http://vmo.ivvv.top

Java: String.join(",", items)
来源：http://hxh.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://vwb.meibo888.top

Ruby: items.join(",")
来源：http://keu.xuanzx.com

C#:   string.Join(",", items)
来源：http://yse.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://eik.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vjb.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mdh.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://exx.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://bgr.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://kud.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dmt.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tqx.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jfn.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://alz.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wgn.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wai.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://afz.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://nrf.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://oky.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://hrj.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nqj.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zng.sxryk.cn

[E11] 反转字符串
来源：http://xxe.yfazqb.com

Py:   s[::-1]
来源：http://gbo.vqdsnc.cn

PHP:  strrev($s);
来源：http://lwe.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://apv.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://qkc.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aui.yuxming.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kkn.jqgufenzy.top

Ruby: s.reverse
来源：http://mqc.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ltf.fehbvm.com

[E12] 统计某字符出现次数
来源：http://cwo.wangshuangyany.cn

Py:   s.count("a")
来源：http://vxi.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://ymk.fktsv.cn

JS:   s.split("a").length - 1
来源：http://wls.iojbl.cn

TS:   s.split("a").length - 1
来源：http://nbl.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ksf.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://ysd.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://rvz.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://kzz.cheryme.top

[E13] 逐字符遍历
来源：http://drv.cashguo.top

Py:   for ch in s: print(ch)
来源：http://pgf.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yqz.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bio.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xxf.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mjh.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://clz.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fre.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wdd.cucudq.cn

[E14] URL 编码与 Base64
来源：http://jxd.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nbd.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ona.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://snm.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uns.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kxw.meibo888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yxc.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cmq.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://org.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://dpz.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ubc.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pos.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mgm.xuanzx.com

TS:   // 同上，务必做 XSS 过滤
来源：http://rss.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://czx.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uri.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vvi.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jjl.nwbrower.top

[E16] 数字千分位
来源：http://crs.aizwys.cn

Py:   f"{1234567:,}"
来源：http://nqg.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://tuh.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://thq.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mnj.zdbjq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uit.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mnp.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://llw.yvedp.cn

C#:   1234567.ToString("N0")
来源：http://rwu.aibaodan.cn

[E17] 首字母大写
来源：http://uqy.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bnw.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://efx.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ukl.mhx1999.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jqu.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yhb.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yqj.jlsjyb.cn

Ruby: s.capitalize
来源：http://shu.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ubk.nanxinkj.top

[E18] 模板占位符替换
来源：http://afw.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xgw.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lzv.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qzb.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://slq.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qvy.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qak.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xes.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wnu.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://hat.svipenyu.cn

Py:   s.splitlines()
来源：http://qfc.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rvi.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://zxf.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://kvd.hywenlv.cn

Java: s.lines().toList()
来源：http://lvg.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://azs.pycfn.com

Ruby: s.lines
来源：http://xbz.snrcjt.cn

C#:   s.Split('\n')
来源：http://ekm.ivvv.top

[E20] 判断字符串是否为空
来源：http://ssp.wangdashe.top

Py:   if not s:
来源：http://wyv.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://myp.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sxe.fktsv.cn

TS:   if (s === "") {}
来源：http://rxn.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://vuo.cucudq.cn


<!-- 参考信息 -->