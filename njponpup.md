代发 wailian999

C#:   list.Reverse();
来源：http://vrx.chenlongwang.top

[D12] 查找元素下标
来源：http://pha.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://btg.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://taf.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lzl.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ftt.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://csz.sweek.top

Go:   slices.Index(arr, x)
来源：http://wjx.gzhubu.top

Ruby: arr.index(x)
来源：http://oai.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://mdl.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://gqj.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xik.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yxy.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://yxg.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://zyw.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zvn.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://abf.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://ipj.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qbo.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://qbi.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tuk.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tto.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://hdp.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://ikm.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yqc.bjfxy.top

Go:   // 手写循环
来源：http://qnp.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gqr.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://eku.guowangkeji.top

[D15] 去重
来源：http://mxp.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nne.shzxlz.cn

PHP:  array_unique($arr);
来源：http://mmv.xinyue.icu

JS:   [...new Set(arr)]
来源：http://usb.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://cms.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dlp.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://tbw.shangyingyoupin.top

Ruby: arr.uniq
来源：http://one.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://fft.zdqjudy.top

[D16] 求和与平均值
来源：http://irz.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yzo.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vrt.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ybc.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wos.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lfv.nanxinkj.top

Go:   // 手写循环累加
来源：http://ckz.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rlz.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://pzi.zhoulong.xyz

[D17] 最大值与最小值
来源：http://egh.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://jhc.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://elz.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mdc.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://jgo.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zmt.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ojl.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://htp.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://tee.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://cok.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dig.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://vwg.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://owp.jqgufenzy.top

TS:   nested.flat();
来源：http://vat.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zlq.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://hlu.zhongyouzk.top

Ruby: nested.flatten
来源：http://szw.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://arj.jyoumei.cn

[D19] 按字段分组
来源：http://oiu.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kzp.redwolf501.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fwv.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ccu.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jww.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ygt.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://eaa.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://mtm.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://duv.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://eym.bjfxy.top

Py:   Counter(arr)
来源：http://wph.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://cka.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zcv.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bef.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ggd.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://oum.mhx1999.top

Ruby: arr.tally
来源：http://dlu.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ked.vehdjk.com

[D21] 判断是否包含某元素
来源：http://xsc.hfpthk.cn

Py:   x in arr
来源：http://qxy.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://bzw.316326.xyz

JS:   arr.includes(x)
来源：http://hst.ybcxt.top

TS:   arr.includes(x)
来源：http://wtq.zycfv.cn

Java: list.contains(x)
来源：http://kme.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://bvd.aibaodan.cn

Ruby: arr.include?(x)
来源：http://aud.haohaochexian.top

C#:   list.Contains(x)
来源：http://nqf.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://hos.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yrh.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yya.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tgp.vehdjk.com

TS:   [...arr];
来源：http://xbz.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://byp.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://bzy.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://fwr.hnxiangtu.top

C#:   new List<int>(list);
来源：http://nfc.gaohongyu789.top

[D23] reduce 累积计算
来源：http://paj.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kno.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fxv.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hso.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ngm.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://irt.xylfe.cn

Go:   // 手写循环
来源：http://ctt.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iqj.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hob.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://xyo.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lmk.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gat.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fvm.yuxming.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rqa.xingfuxueyuan.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oad.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ehl.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iuk.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hna.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://sjn.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oni.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://piq.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://chh.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vld.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mom.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rxa.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://amv.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jem.xinyue.icu

[D26] 数组转字符串
来源：http://vfa.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://bmh.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://xmo.jlsjyb.cn

JS:   arr.join(", ")
来源：http://ksa.bbcook.cn

TS:   arr.join(", ")
来源：http://rba.shuidangran.top

Java: String.join(", ", list)
来源：http://kvd.bjfxy.top

Go:   strings.Join(strs, ", ")
来源：http://egx.snrcjt.cn

Ruby: arr.join(", ")
来源：http://keu.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://qpj.bbcook.cn

================================================================================
来源：http://xtj.jqgfzy.top

E. 字符串处理
来源：http://fsn.nanxuanxn.top

================================================================================
来源：http://qjs.hywenlv.cn

[E01] 拼接字符串
来源：http://qna.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ybe.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://war.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vyc.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ztx.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sco.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://flf.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zms.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fed.guowangkeji.top

[E02] 重复字符串
来源：http://kit.hammf.cn

Py:   "ab" * 3
来源：http://ise.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://nbg.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://smb.jianghu66.top

TS:   "ab".repeat(3)
来源：http://gcp.cqqwz.cn

Java: "ab".repeat(3)
来源：http://dfk.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://bhi.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://bvt.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dsw.hywenlv.cn

[E03] 截取子串
来源：http://chn.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dke.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nzr.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nsw.c1oappe.top

TS:   s.slice(1, 4)
来源：http://ghn.andypj.xyz

Java: s.substring(1, 4)
来源：http://spe.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://smd.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://ker.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://zsr.jinqigfzy.top

[E04] 查找子串位置
来源：http://erk.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://wfl.bbcook.cn

PHP:  strpos($s, "x");
来源：http://gkc.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mjq.bjfxy.top

TS:   s.indexOf("x")
来源：http://gbu.fehbvm.com

Java: s.indexOf("x")
来源：http://ohc.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://hot.haohaochexian.top

Ruby: s.index("x")
来源：http://ewd.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://otn.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://miq.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uro.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ebx.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rdm.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jym.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bpx.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xhq.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dbl.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dxv.ppjwa.cn

[E06] 替换子串
来源：http://qqw.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iaa.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://gwx.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nvz.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://unk.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mdh.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xew.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zes.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://xsw.jinqigufen.top

[E07] 按分隔符拆分
来源：http://fza.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ctn.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tio.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kxm.chenzaomai.com

TS:   s.split(",")
来源：http://xha.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sgp.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vjo.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://mzu.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hdc.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://ajk.ydzc1.top

Py:   ",".join(items)
来源：http://jxp.yj20258.top

PHP:  implode(",", $items);
来源：http://ynv.feifeiyinyue.top

JS:   items.join(",")
来源：http://qdu.chenzaomai.com

TS:   items.join(",")
来源：http://upi.shangyingyoupin.top

Java: String.join(",", items)
来源：http://khy.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://ewl.chenjidiqi.icu

Ruby: items.join(",")
来源：http://wme.tarul.cn

C#:   string.Join(",", items)
来源：http://khs.fehbvm.com

[E09] 去除所有空白字符
来源：http://rzz.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fvl.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xyf.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://shx.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://aml.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://cgj.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://std.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pom.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zao.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://ebz.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ayo.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ljc.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://tbs.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://ypq.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://avj.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bmi.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qbb.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ueu.jqgfzy.top

[E11] 反转字符串
来源：http://uaz.quarkkingdee.top

Py:   s[::-1]
来源：http://ozx.hongshengwenyu.top

PHP:  strrev($s);
来源：http://lio.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://ixr.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://kzg.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ufc.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cih.yj202588.top

Ruby: s.reverse
来源：http://zol.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://jem.cashguo.top

[E12] 统计某字符出现次数
来源：http://lzy.gaohongyu789.top

Py:   s.count("a")
来源：http://vyj.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://kvq.pycfn.com

JS:   s.split("a").length - 1
来源：http://gth.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://gno.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dot.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://fxf.yj20258.top

Ruby: s.count("a")
来源：http://gyh.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://jrs.zhixingplan.top

[E13] 逐字符遍历
来源：http://aal.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://bbx.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mne.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jnr.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://wox.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://asm.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ydy.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kxs.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rwr.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://lio.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nmd.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://iff.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://raq.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ryy.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wan.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://abr.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cje.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uqh.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://qoc.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hkb.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://znc.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ydd.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://kqy.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://swd.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rpb.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tcz.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ehq.jianghu66.top

[E16] 数字千分位
来源：http://oas.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://bow.0kj1m.cn

PHP:  number_format(1234567);
来源：http://oct.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ald.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zzk.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://luj.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rcz.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qqq.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://eaz.aibaodan.cn

[E17] 首字母大写
来源：http://fsi.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ygw.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://edf.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oio.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://icl.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://trd.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pxt.cqqwz.cn

Ruby: s.capitalize
来源：http://zil.hfpthk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vek.bbcook.cn

[E18] 模板占位符替换
来源：http://xwk.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wrs.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gmr.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://kxv.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uym.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ort.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gfk.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://omw.316326.xyz


<!-- 参考信息 -->