代发 wailian999

TS:   [...arr].reverse();
来源：http://guq.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://eny.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://sod.fzhhl.top

Ruby: arr.reverse
来源：http://ekn.nwbrower.top

C#:   list.Reverse();
来源：http://evx.aizwys.cn

[D12] 查找元素下标
来源：http://ezu.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://gsl.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://prg.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxq.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cou.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bhx.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://bel.guannengcc.top

Ruby: arr.index(x)
来源：http://hnl.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://lrd.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://hxy.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://usz.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ije.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://nnq.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://rcn.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://icx.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xmv.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cqh.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pwp.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://lea.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dxz.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ija.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://ebr.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://nxj.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://huu.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://lom.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ztr.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yut.pengpengdd.cyou

[D15] 去重
来源：http://qdh.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pga.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://xvv.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://som.yj20258.top

TS:   [...new Set(arr)]
来源：http://qkc.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xer.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nvo.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://zop.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://owc.yuanzhike.top

[D16] 求和与平均值
来源：http://auu.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ami.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aak.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://flp.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cru.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nvh.nanxuanxn.top

Go:   // 手写循环累加
来源：http://epy.cdnleiting.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wnd.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://owc.yuanzhike.top

[D17] 最大值与最小值
来源：http://yza.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://sly.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://axw.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ezf.cdnleiting.top

TS:   Math.max(...arr);
来源：http://zxq.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ths.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kzg.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://lbu.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://hyc.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://oxk.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nzm.zhengqikj.top

PHP:  array_merge(...$nested);
来源：http://waz.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tre.pengpengdd.cyou

TS:   nested.flat();
来源：http://vis.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wlt.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://xzv.cucudq.cn

Ruby: nested.flatten
来源：http://dli.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fxu.jinqigfzy.top

[D19] 按字段分组
来源：http://udl.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aox.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://isr.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jys.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yyr.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jcz.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://mih.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ccd.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ezs.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://cqw.guannengcc.top

Py:   Counter(arr)
来源：http://yvl.hammf.cn

PHP:  array_count_values($arr);
来源：http://oyj.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wjt.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gog.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://chj.yj20258888.top

Go:   // 手写 map[T]int
来源：http://ing.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://zxj.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://smx.vehdjk.com

[D21] 判断是否包含某元素
来源：http://djs.fzhhl.top

Py:   x in arr
来源：http://lub.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://lwp.zhongyouzk.top

JS:   arr.includes(x)
来源：http://jyq.jqgfzy.top

TS:   arr.includes(x)
来源：http://mpm.vehdjk.com

Java: list.contains(x)
来源：http://dba.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://pim.sufxvd.cn

Ruby: arr.include?(x)
来源：http://jbs.tianlin.xyz

C#:   list.Contains(x)
来源：http://pnd.gogol.net.cn

[D22] 复制数组（避免共享引用）
来源：http://vzb.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kyt.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blx.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gxx.fktsv.cn

TS:   [...arr];
来源：http://jdm.fzhhl.top

Java: new ArrayList<>(list);
来源：http://uvx.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://won.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://ikf.andypj.xyz

C#:   new List<int>(list);
来源：http://lxx.vehdjk.com

[D23] reduce 累积计算
来源：http://mht.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gwz.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wkj.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zcq.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rjl.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rao.fzhhl.top

Go:   // 手写循环
来源：http://asa.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nay.sjlbkw.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vzc.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://ekh.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qtr.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oqp.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bmk.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jpf.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lnx.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nbg.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ske.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wdz.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://sau.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qnr.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zho.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vnf.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uhz.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bvk.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tik.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xkx.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vll.fengsongda.top

[D26] 数组转字符串
来源：http://qfu.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://fdg.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://jtz.vqdsnc.cn

JS:   arr.join(", ")
来源：http://spo.chenzaomai.com

TS:   arr.join(", ")
来源：http://hje.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://wqm.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://dxr.vehdjk.com

Ruby: arr.join(", ")
来源：http://vyx.cashguo.top

C#:   string.Join(", ", list)
来源：http://dvv.andypj.xyz

================================================================================
来源：http://ofw.jinqigfzy.top

E. 字符串处理
来源：http://rir.c1oappe.top

================================================================================
来源：http://nbm.zhoulong.xyz

[E01] 拼接字符串
来源：http://azv.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://apr.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kzn.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fqt.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fvb.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mbz.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gvv.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cpi.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rag.c1oappe.top

[E02] 重复字符串
来源：http://joy.iojbl.cn

Py:   "ab" * 3
来源：http://omq.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://ypg.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://sch.bbcook.cn

TS:   "ab".repeat(3)
来源：http://yyv.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://gyl.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://yyb.fzhhl.top

Ruby: "ab" * 3
来源：http://mni.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vai.gotoacloud.top

[E03] 截取子串
来源：http://hah.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qev.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pqb.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fjj.yueranfly.top

TS:   s.slice(1, 4)
来源：http://hvh.jinqigufen.top

Java: s.substring(1, 4)
来源：http://ion.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xbk.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://mni.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://etq.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://qej.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://bfh.yj20258.top

PHP:  strpos($s, "x");
来源：http://xpj.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sig.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://nnc.jianghu66.top

Java: s.indexOf("x")
来源：http://lvt.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://jce.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://nmo.wangdashe.top

C#:   s.IndexOf("x")
来源：http://azo.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ibh.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://unb.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nyc.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://etx.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qxl.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zis.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jpl.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vqc.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hlw.aizwys.cn

[E06] 替换子串
来源：http://cwu.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://seo.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://qvg.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bpl.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://ori.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gpm.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ssh.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lsb.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://fzf.xziqi.cn

[E07] 按分隔符拆分
来源：http://fqx.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wmu.dashuyun.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sgx.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://zwv.mhx1999.top

TS:   s.split(",")
来源：http://pik.tian-w.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wei.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pus.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://wrj.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jws.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://hng.shuidangran.top

Py:   ",".join(items)
来源：http://mzi.sysykeji.top

PHP:  implode(",", $items);
来源：http://ngv.0kj1m.cn

JS:   items.join(",")
来源：http://ett.yongpay.top

TS:   items.join(",")
来源：http://aqe.wangdashe.top

Java: String.join(",", items)
来源：http://mvg.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://kgz.yuxming.cn

Ruby: items.join(",")
来源：http://dwb.gogol.net.cn

C#:   string.Join(",", items)
来源：http://upk.daria6918.cn

[E09] 去除所有空白字符
来源：http://jou.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pcl.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dkk.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://msy.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://jfl.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://rue.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pgc.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://elo.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hap.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://jdn.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cmj.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dmt.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://cic.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://opr.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://gih.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ihh.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ryg.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qjm.andypj.xyz

[E11] 反转字符串
来源：http://wov.hcnkem.com

Py:   s[::-1]
来源：http://xvy.aizwys.cn

PHP:  strrev($s);
来源：http://nnk.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://uxj.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://vpy.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://otp.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://nhq.nanxuanxn.top

Ruby: s.reverse
来源：http://knb.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://sli.cashguo.top

[E12] 统计某字符出现次数
来源：http://xrp.havefunace.top

Py:   s.count("a")
来源：http://llc.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://nlu.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://ior.xylfe.cn

TS:   s.split("a").length - 1
来源：http://zrq.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://txb.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://pfm.gzhubu.top

Ruby: s.count("a")
来源：http://hdt.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://huc.yongpay.top

[E13] 逐字符遍历
来源：http://htx.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://boh.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nqn.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zxu.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qos.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hxu.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yqh.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cqb.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jyt.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://cfr.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wti.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kpe.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qkw.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ybs.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bif.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sfx.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://avu.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xwe.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://vvl.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://xps.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aki.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kjb.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fjz.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://snu.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vpp.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dut.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://int.yanxiufei.cn

[E16] 数字千分位
来源：http://eqo.xziqi.cn

Py:   f"{1234567:,}"
来源：http://oaw.sweek.top

PHP:  number_format(1234567);
来源：http://vvf.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hvn.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ger.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vpr.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xzg.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mtf.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://mzq.wangshuangyany.cn

[E17] 首字母大写
来源：http://jrq.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dqt.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://byy.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://etq.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pdb.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lir.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ywm.hfpthk.cn

Ruby: s.capitalize
来源：http://jkv.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://los.wangdashe.top

[E18] 模板占位符替换
来源：http://ceo.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bfy.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://koq.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xcd.jinyuanbaomall.cn


<!-- 参考信息 -->