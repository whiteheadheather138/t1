代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://jvx.jlsjyb.cn

Go:   // 手写循环
来源：http://vch.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bdj.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ado.jqgufenzy.top

[D15] 去重
来源：http://nzt.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ego.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://fnu.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://gcl.havefunace.top

TS:   [...new Set(arr)]
来源：http://glt.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ivo.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://izb.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://ozm.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://vhz.pycfn.com

[D16] 求和与平均值
来源：http://qvy.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tcd.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qtf.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sqa.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://anp.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://arn.svipenyu.cn

Go:   // 手写循环累加
来源：http://lvb.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iej.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://dmf.316326.xyz

[D17] 最大值与最小值
来源：http://hfp.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://lnn.tianlin.xyz

PHP:  max($arr);  min($arr);
来源：http://frp.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nnf.zhixingplan.top

TS:   Math.max(...arr);
来源：http://zdt.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dea.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xjv.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://cfg.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://dpd.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://spy.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rjc.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://gmu.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qxj.epnwcf.com

TS:   nested.flat();
来源：http://wzq.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ikq.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://soc.yuanzhike.top

Ruby: nested.flatten
来源：http://xts.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wuz.dianchejie.cn

[D19] 按字段分组
来源：http://gph.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ecc.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hup.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cma.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pfs.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zaw.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://hrh.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://slf.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://unx.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://cnu.sufxvd.cn

Py:   Counter(arr)
来源：http://vdm.xziqi.cn

PHP:  array_count_values($arr);
来源：http://gnm.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xzc.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eje.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iew.hesvh.cn

Go:   // 手写 map[T]int
来源：http://kec.xylfe.cn

Ruby: arr.tally
来源：http://liq.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qxj.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://sue.xziqi.cn

Py:   x in arr
来源：http://umh.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://zpb.nwbrower.top

JS:   arr.includes(x)
来源：http://njx.dashuyun.cn

TS:   arr.includes(x)
来源：http://dyl.jinqigufen.top

Java: list.contains(x)
来源：http://yje.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://itb.jinqigufen.top

Ruby: arr.include?(x)
来源：http://ivc.yueranfly.top

C#:   list.Contains(x)
来源：http://vum.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://atm.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fsf.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fqo.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cka.jinqigfzy.top

TS:   [...arr];
来源：http://lca.hcnkem.com

Java: new ArrayList<>(list);
来源：http://rmv.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ykz.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://ucs.mhx1999.top

C#:   new List<int>(list);
来源：http://ioo.zdqjudy.top

[D23] reduce 累积计算
来源：http://etp.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mvb.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zzz.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tql.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yoe.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uqo.fengsongda.top

Go:   // 手写循环
来源：http://rzq.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hzp.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qns.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://pyf.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://msi.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nyt.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ydq.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jtj.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wkb.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pax.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cfw.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ore.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://cnc.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nps.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eti.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://euj.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oky.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sdf.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://elr.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://klp.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cus.jinqigufen.top

[D26] 数组转字符串
来源：http://itj.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://fge.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://umk.kuanghao11.cn

JS:   arr.join(", ")
来源：http://sir.gotoacloud.top

TS:   arr.join(", ")
来源：http://soh.fktsv.cn

Java: String.join(", ", list)
来源：http://cgy.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://wtv.vehdjk.com

Ruby: arr.join(", ")
来源：http://zkp.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://oec.zycfv.cn

================================================================================
来源：http://xcu.jinqigufen.top

E. 字符串处理
来源：http://unm.9152youxi.cn

================================================================================
来源：http://lkw.pengpengdd.cyou

[E01] 拼接字符串
来源：http://igq.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fxj.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zzo.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iuj.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mig.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bwq.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://awt.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lvo.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hja.svipenyu.cn

[E02] 重复字符串
来源：http://xvo.yfazqb.com

Py:   "ab" * 3
来源：http://iny.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://byu.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://sdh.mhx1999.top

TS:   "ab".repeat(3)
来源：http://haf.tianlin.xyz

Java: "ab".repeat(3)
来源：http://hal.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://pvk.shuidangran.top

Ruby: "ab" * 3
来源：http://wdp.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://alk.fktsv.cn

[E03] 截取子串
来源：http://kzn.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yof.zdbjq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wnj.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vrc.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://itp.havefunace.top

Java: s.substring(1, 4)
来源：http://pne.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kmd.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://atn.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://qlc.chenzaomai.com

[E04] 查找子串位置
来源：http://jud.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://ytk.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://mtw.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rlm.tian-w.cn

TS:   s.indexOf("x")
来源：http://lci.xinyue.icu

Java: s.indexOf("x")
来源：http://hzo.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://udx.hongshengwenyu.top

Ruby: s.index("x")
来源：http://xpj.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://zjj.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mkh.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zxl.yj20258888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bua.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uyd.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://yjv.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tul.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sxb.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xzm.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hgu.hcnkem.com

[E06] 替换子串
来源：http://mxi.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qkr.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://boo.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uvo.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://tih.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cnh.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vao.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gmf.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://mvb.mhx1999.top

[E07] 按分隔符拆分
来源：http://iya.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yea.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gvx.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vuo.ydjk.org.cn

TS:   s.split(",")
来源：http://wvs.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bnj.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://duw.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://afj.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://upb.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://jdt.xuanzx.com

Py:   ",".join(items)
来源：http://tds.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://nei.yvedp.cn

JS:   items.join(",")
来源：http://ojl.iojbl.cn

TS:   items.join(",")
来源：http://qed.sjlbkw.cn

Java: String.join(",", items)
来源：http://erp.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://isc.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://vhj.c1oappe.top

C#:   string.Join(",", items)
来源：http://pkp.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://nxj.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ona.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lhw.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://yel.yj20258888.top

TS:   s.replace(/\s+/g, "")
来源：http://vzh.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://wjz.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xmt.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mqw.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fal.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://cyv.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sba.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qzs.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://lgy.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://dgs.yueranfly.top

Java: String.format("%03d", 7)
来源：http://zaq.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rkh.yongpay.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zgb.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tfz.daria6918.cn

[E11] 反转字符串
来源：http://bxr.nanxinkj.top

Py:   s[::-1]
来源：http://kav.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://kjh.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://ruk.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://rhf.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iaj.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pxi.gzhubu.top

Ruby: s.reverse
来源：http://alq.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://krd.sxryk.cn

[E12] 统计某字符出现次数
来源：http://jvg.hongshengwenyu.top

Py:   s.count("a")
来源：http://cgp.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://gcy.ydzc1.top

JS:   s.split("a").length - 1
来源：http://qwj.jianghu66.top

TS:   s.split("a").length - 1
来源：http://bzr.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eus.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://izv.ivvv.top

Ruby: s.count("a")
来源：http://pye.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://pef.zhongyouzk.top

[E13] 逐字符遍历
来源：http://bjq.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://eio.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iad.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hqe.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bfm.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gbw.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nih.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://web.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://amm.yfazqb.com

[E14] URL 编码与 Base64
来源：http://kgc.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fzc.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gep.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://srb.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wvm.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yms.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vht.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gzj.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vdw.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://rpk.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://rfo.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mip.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kxr.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iit.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qcm.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aha.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gma.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jop.jinqigfzy.top

[E16] 数字千分位
来源：http://lxt.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://vwf.ppjwa.cn

PHP:  number_format(1234567);
来源：http://hcb.hysaishi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nod.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ehe.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wxd.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pfl.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://exd.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://clm.zhixingplan.top

[E17] 首字母大写
来源：http://qft.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dwr.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://net.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ddx.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nwy.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cvr.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sob.hongshengwenyu.top

Ruby: s.capitalize
来源：http://gnz.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lry.yonumen.top

[E18] 模板占位符替换
来源：http://qzj.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cko.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uhh.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sjx.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qlu.jqgufenzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vhf.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yzi.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://exg.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gny.shuidangran.top

[E19] 多行文本按行拆分
来源：http://nsp.wangdashe.top

Py:   s.splitlines()
来源：http://huh.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rew.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://eev.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://epv.ivvv.top

Java: s.lines().toList()
来源：http://mnd.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://mrh.jinqigfzy.top

Ruby: s.lines
来源：http://vuh.nanxinkj.top

C#:   s.Split('\n')
来源：http://okx.xuanzx.com

[E20] 判断字符串是否为空
来源：http://waz.zdqjudy.top

Py:   if not s:
来源：http://fxf.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mib.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sas.zhengqikj.top

TS:   if (s === "") {}
来源：http://vas.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://hoj.daria6918.cn

Go:   if s == "" {}
来源：http://pwx.yangfankeji.com

Ruby: if s.empty?
来源：http://zhq.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kiq.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://xhh.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ayx.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rqw.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nnf.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bmt.hongshengwenyu.top


<!-- 参考信息 -->