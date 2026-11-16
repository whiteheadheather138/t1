代发 wailian999

TS:   [...arr].reverse();
来源：http://kls.xylfe.cn

Java: Collections.reverse(list);
来源：http://bxq.316326.xyz

Go:   slices.Reverse(arr)
来源：http://xvo.aizwys.cn

Ruby: arr.reverse
来源：http://anv.iojbl.cn

C#:   list.Reverse();
来源：http://cwc.bjfxy.top

[D12] 查找元素下标
来源：http://qvj.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://yvx.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hab.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ysh.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iff.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fvm.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://iru.zycfv.cn

Ruby: arr.index(x)
来源：http://lob.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://kln.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://zce.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jek.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kyw.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://vrv.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://fdg.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wiy.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://moe.daxiang520.top

Ruby: arr.select { |x| x > 3 }
来源：http://hkp.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://arc.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://ivu.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gac.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vbc.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://rsu.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://bpn.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://frs.jinghuilouyu.cn

Go:   // 手写循环
来源：http://fmg.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dhn.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yza.shanyushiyangkeji.top

[D15] 去重
来源：http://kzy.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://edi.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://fmd.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://mqa.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://zuq.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lss.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://alu.dianchejie.cn

Ruby: arr.uniq
来源：http://koz.meibo888.top

C#:   list.Distinct().ToList()
来源：http://nbg.wangshuangyany.cn

[D16] 求和与平均值
来源：http://qvu.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mzp.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nqc.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqi.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lxb.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xxn.xziqi.cn

Go:   // 手写循环累加
来源：http://eaj.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://agb.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://oam.sysykeji.top

[D17] 最大值与最小值
来源：http://xlr.tarul.cn

Py:   max(arr);  min(arr)
来源：http://rmx.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://imi.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zpu.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://beu.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ali.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fmk.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://evy.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://vfy.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://nml.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mdt.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://tts.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bbx.ppjwa.cn

TS:   nested.flat();
来源：http://cnp.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jpy.meibo888.top

Go:   // 手写双层循环
来源：http://smd.iojbl.cn

Ruby: nested.flatten
来源：http://wqd.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ypk.zhengqikj.top

[D19] 按字段分组
来源：http://miu.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://thi.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rns.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xxs.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://upa.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cov.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://tag.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://osr.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mme.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://vlp.yanxiufei.cn

Py:   Counter(arr)
来源：http://qna.wangdashe.top

PHP:  array_count_values($arr);
来源：http://iuv.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uup.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kop.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qdk.cheryme.top

Go:   // 手写 map[T]int
来源：http://rks.gzhubu.top

Ruby: arr.tally
来源：http://ehd.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zpn.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://sdy.redwolf501.top

Py:   x in arr
来源：http://jco.chenjidiqi.icu

PHP:  in_array($x, $arr, true);
来源：http://fqy.sweek.top

JS:   arr.includes(x)
来源：http://her.mhx1999.top

TS:   arr.includes(x)
来源：http://cet.daxiang520.top

Java: list.contains(x)
来源：http://bia.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://mfx.vehdjk.com

Ruby: arr.include?(x)
来源：http://lhr.vehdjk.com

C#:   list.Contains(x)
来源：http://fxi.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://hfq.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lws.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gen.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hml.sxryk.cn

TS:   [...arr];
来源：http://qsm.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://ijs.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://psj.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://mnn.yongpay.top

C#:   new List<int>(list);
来源：http://ops.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://haf.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ico.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://khk.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cfy.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mmu.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://utg.tian-w.cn

Go:   // 手写循环
来源：http://fjr.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qxc.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lpx.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://wio.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bzu.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://clk.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wzt.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bxx.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mpz.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kmu.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://erh.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://apo.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://kot.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://afj.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://soo.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jhd.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tbo.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ghd.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mid.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://shn.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gqk.jinqigfzy.top

[D26] 数组转字符串
来源：http://agx.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://fbp.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://jax.aibaodan.cn

JS:   arr.join(", ")
来源：http://vij.ybcxt.top

TS:   arr.join(", ")
来源：http://xqf.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://pfi.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://dsi.shuidangran.top

Ruby: arr.join(", ")
来源：http://rpq.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://rvd.tianlin.xyz

================================================================================
来源：http://twe.dashuyun.cn

E. 字符串处理
来源：http://xvw.fengsongda.top

================================================================================
来源：http://wte.shanyushiyangtech.top

[E01] 拼接字符串
来源：http://tws.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iax.shuidangran.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wfg.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://for.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://deu.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uxe.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://scf.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cuv.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://elc.fktsv.cn

[E02] 重复字符串
来源：http://fjj.fengsongda.top

Py:   "ab" * 3
来源：http://usd.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://iyp.xinyue.icu

JS:   "ab".repeat(3)
来源：http://xqh.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://iwj.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://xba.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://ckx.dashuyun.cn

Ruby: "ab" * 3
来源：http://oxb.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kkj.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://wph.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lyv.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ofj.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ocx.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://apc.sweek.top

Java: s.substring(1, 4)
来源：http://jal.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zru.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://fmp.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://ygk.yuxming.cn

[E04] 查找子串位置
来源：http://jgz.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://xbb.wangdashe.top

PHP:  strpos($s, "x");
来源：http://xbi.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://avx.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://dpg.svipenyu.cn

Java: s.indexOf("x")
来源：http://snc.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://vsa.hongshengwenyu.top

Ruby: s.index("x")
来源：http://hmx.nwbrower.top

C#:   s.IndexOf("x")
来源：http://fzb.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://opl.nwbrower.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rql.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kzj.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upe.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fgl.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ayd.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tfo.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://une.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ysa.tanke756.top

[E06] 替换子串
来源：http://qbh.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jsm.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://rix.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lnc.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://psj.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ktm.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tjq.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cga.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://kjv.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://xnx.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qsm.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ptf.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uby.tarul.cn

TS:   s.split(",")
来源：http://hzc.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://inm.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tdo.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://dge.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kvn.smart0.xyz

[E08] 数组按分隔符合并
来源：http://ghn.sjlbkw.cn

Py:   ",".join(items)
来源：http://bsd.yuanzhike.top

PHP:  implode(",", $items);
来源：http://hdg.0kj1m.cn

JS:   items.join(",")
来源：http://atd.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://ezn.andypj.xyz

Java: String.join(",", items)
来源：http://eff.chenlongwang.top

Go:   strings.Join(items, ",")
来源：http://xzb.fktsv.cn

Ruby: items.join(",")
来源：http://rto.zdqjudy.top

C#:   string.Join(",", items)
来源：http://arg.hysaishi.cn

[E09] 去除所有空白字符
来源：http://kbv.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hgb.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ysc.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://myz.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://ppl.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://ouf.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mqv.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tci.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://imn.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://rpo.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pya.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ztl.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://uri.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://kml.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://jmm.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ihq.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rqa.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mnv.jinqigfzy.top

[E11] 反转字符串
来源：http://frk.pycfn.com

Py:   s[::-1]
来源：http://tfd.yuxming.cn

PHP:  strrev($s);
来源：http://nsn.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://ufg.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://iyq.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://voc.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xcy.redwolf501.top

Ruby: s.reverse
来源：http://mfr.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eim.yvedp.cn

[E12] 统计某字符出现次数
来源：http://tfy.yj20258888.top

Py:   s.count("a")
来源：http://jyf.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://fsv.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://hev.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://ecy.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tcg.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://rax.hcnkem.com

Ruby: s.count("a")
来源：http://zhe.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://olh.fanxiaobao.xyz

[E13] 逐字符遍历
来源：http://pix.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://azo.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dje.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cid.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lav.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ozg.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cfj.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qje.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ndk.aizwys.cn

[E14] URL 编码与 Base64
来源：http://cav.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://swr.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qta.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iou.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vee.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://igo.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gav.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ssw.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fhp.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://czs.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ool.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ktg.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ywi.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wqk.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yhh.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gdg.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qzz.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jds.cucudq.cn

[E16] 数字千分位
来源：http://fyn.yuxming.cn

Py:   f"{1234567:,}"
来源：http://sdr.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://yiy.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://muf.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wka.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rez.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zau.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tqi.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://ggj.gzhubu.top

[E17] 首字母大写
来源：http://ate.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://buw.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gyg.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oir.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nmz.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xbj.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rgd.sufxvd.cn

Ruby: s.capitalize
来源：http://hyo.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://you.smart0.xyz

[E18] 模板占位符替换
来源：http://edq.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://puq.wangshuangyany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://owf.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nla.ybcxt.top


<!-- 参考信息 -->