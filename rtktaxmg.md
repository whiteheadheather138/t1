代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://avq.yj20258.top

Go:   // 手写循环
来源：http://sos.daxiang520.top

Ruby: arr.map { |x| x * 2 }
来源：http://faj.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ccq.tian-w.cn

[D15] 去重
来源：http://ecb.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aaa.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://vtr.yj20258.top

JS:   [...new Set(arr)]
来源：http://rib.daxiang520.top

TS:   [...new Set(arr)]
来源：http://xom.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tjm.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xea.sysykeji.top

Ruby: arr.uniq
来源：http://wtt.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://ckx.cqqwz.cn

[D16] 求和与平均值
来源：http://mof.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vje.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rks.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iup.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bxx.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nag.cucudq.cn

Go:   // 手写循环累加
来源：http://kue.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nqq.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://kcm.yj20258.top

[D17] 最大值与最小值
来源：http://rew.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://djj.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://nki.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dmb.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://lox.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://nvg.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://alu.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://dxs.yj20258.top

C#:   list.Max();  list.Min()
来源：http://pvn.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://cxx.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rld.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://hlg.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dcw.guannengcc.top

TS:   nested.flat();
来源：http://fle.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://onl.tanke756.top

Go:   // 手写双层循环
来源：http://olx.chenlongwang.top

Ruby: nested.flatten
来源：http://mqs.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jgv.jianghu66.top

[D19] 按字段分组
来源：http://wqc.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ixy.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jke.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gct.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://csn.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rkd.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://isa.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://gcb.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yxy.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://xyv.fehbvm.com

Py:   Counter(arr)
来源：http://iup.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://rlq.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bia.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://naz.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hkf.birdmap.top

Go:   // 手写 map[T]int
来源：http://jbd.yj20258888.top

Ruby: arr.tally
来源：http://lbj.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://arw.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://dun.c1oappe.top

Py:   x in arr
来源：http://nhj.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://rym.hammf.cn

JS:   arr.includes(x)
来源：http://wtf.9152youxi.cn

TS:   arr.includes(x)
来源：http://juc.chenzaomai.com

Java: list.contains(x)
来源：http://xij.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://guf.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://doz.birdmap.top

C#:   list.Contains(x)
来源：http://cxx.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://dpn.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oje.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://agn.havefunace.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ntw.zhiwuduotai.top

TS:   [...arr];
来源：http://sve.aizwys.cn

Java: new ArrayList<>(list);
来源：http://mwa.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://zzl.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://iob.dianchejie.cn

C#:   new List<int>(list);
来源：http://fuv.yueranfly.top

[D23] reduce 累积计算
来源：http://fsz.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zii.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qmb.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xer.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yrc.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ofj.pycfn.com

Go:   // 手写循环
来源：http://eaj.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dvc.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://thy.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://mlw.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ayw.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mdn.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lto.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pnf.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lxj.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uaf.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://smv.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ozn.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://uts.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mvq.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dmo.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uqs.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lob.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xju.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dvb.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nac.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sva.ehwqpu.com

[D26] 数组转字符串
来源：http://sdf.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://dkz.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://ath.aizwys.cn

JS:   arr.join(", ")
来源：http://tev.nanxinkj.top

TS:   arr.join(", ")
来源：http://aro.cheryme.top

Java: String.join(", ", list)
来源：http://uwf.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://sde.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://aam.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://yla.dashuyun.cn

================================================================================
来源：http://zrd.fanxiaobao.xyz

E. 字符串处理
来源：http://evi.zhaomingkeji.xyz

================================================================================
来源：http://kxd.fktsv.cn

[E01] 拼接字符串
来源：http://itk.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://orw.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qmr.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://stg.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqg.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fbd.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pqd.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qqz.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pki.hysaishi.cn

[E02] 重复字符串
来源：http://amo.jqgufenzy.top

Py:   "ab" * 3
来源：http://bhk.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://jmm.ydzc1.top

JS:   "ab".repeat(3)
来源：http://hkq.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://cdv.zdqjudy.top

Java: "ab".repeat(3)
来源：http://pdq.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://zod.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://jcx.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fcn.wangshuangyany.cn

[E03] 截取子串
来源：http://jph.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hon.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cve.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ykp.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://cpl.hywenlv.cn

Java: s.substring(1, 4)
来源：http://qqp.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eqn.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bgz.uphjek.com

C#:   s.Substring(1, 3)
来源：http://sxw.yfazqb.com

[E04] 查找子串位置
来源：http://mnj.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://mrq.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://kfk.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://alz.sweek.top

TS:   s.indexOf("x")
来源：http://hzd.chenlongwang.top

Java: s.indexOf("x")
来源：http://vhl.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://vvp.yfazqb.com

Ruby: s.index("x")
来源：http://emx.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://dmu.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zkj.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ylj.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jmq.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jaw.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iyj.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tby.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hgd.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vcr.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wwe.zhongyouzk.top

[E06] 替换子串
来源：http://adr.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lwx.9152youxi.cn

PHP:  str_replace("a", "b", $s);
来源：http://uzc.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://evm.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://hft.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zlc.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ntm.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zjd.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://xob.andypj.xyz

[E07] 按分隔符拆分
来源：http://roz.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qiy.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vyq.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dgh.yonumen.top

TS:   s.split(",")
来源：http://jrs.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vkj.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cuu.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://idv.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://krp.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://rvu.hfpthk.cn

Py:   ",".join(items)
来源：http://neh.52xcode.cn

PHP:  implode(",", $items);
来源：http://jcq.xuanzx.com

JS:   items.join(",")
来源：http://ahu.nanxinkj.top

TS:   items.join(",")
来源：http://sri.hongshengwenyu.top

Java: String.join(",", items)
来源：http://bcg.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://qih.xziqi.cn

Ruby: items.join(",")
来源：http://pvu.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://fmt.zycfv.cn

[E09] 去除所有空白字符
来源：http://jhg.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fsi.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xsn.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://ift.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://zga.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://syw.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ujr.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ibe.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://olz.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://xoh.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dgr.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://knz.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://ouc.yanxiufei.cn

TS:   "7".padStart(3, "0")
来源：http://yin.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://xxu.birdmap.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aaj.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iqi.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zlw.tian-w.cn

[E11] 反转字符串
来源：http://kdx.nanxuanxn.top

Py:   s[::-1]
来源：http://gzw.xuanzx.com

PHP:  strrev($s);
来源：http://evq.tarul.cn

JS:   [...s].reverse().join("")
来源：http://oan.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://fkz.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wvq.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rjx.tanke756.top

Ruby: s.reverse
来源：http://wim.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://qik.ybcxt.top

[E12] 统计某字符出现次数
来源：http://cul.hongshengwenyu.top

Py:   s.count("a")
来源：http://pag.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://fec.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://xvt.wangdashe.top

TS:   s.split("a").length - 1
来源：http://oux.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ial.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://hpi.daxiang520.top

Ruby: s.count("a")
来源：http://tfa.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://cmk.ehwqpu.com

[E13] 逐字符遍历
来源：http://vnv.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://xpl.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iao.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pcm.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hco.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wih.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kdx.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nhq.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wxq.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://riz.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wzc.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dfj.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jkd.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jyu.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zsq.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ntf.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ytj.haohaochexian.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ose.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://fhi.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://srs.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tsh.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pfj.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://omx.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cgq.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qdr.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kqx.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vxb.mhx1999.top

[E16] 数字千分位
来源：http://qaf.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://igf.ivvv.top

PHP:  number_format(1234567);
来源：http://zmt.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uqa.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ptq.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://urw.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mza.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lth.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://gkw.cashguo.top

[E17] 首字母大写
来源：http://rut.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zda.yonumen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ptg.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://waa.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qme.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pwh.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rlt.zhengqikj.top

Ruby: s.capitalize
来源：http://wns.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rsk.bjfxy.top

[E18] 模板占位符替换
来源：http://krl.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jfk.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xne.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://lun.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ukp.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ctm.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gjk.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rmz.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bru.tian-w.cn

[E19] 多行文本按行拆分
来源：http://zih.zycfv.cn

Py:   s.splitlines()
来源：http://pnk.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nid.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://zjt.hywenlv.cn

TS:   s.split(/\r?\n/)
来源：http://uqm.pycfn.com

Java: s.lines().toList()
来源：http://oov.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://bms.hysaishi.cn

Ruby: s.lines
来源：http://ieq.zdqjudy.top

C#:   s.Split('\n')
来源：http://vvy.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://plf.hywenlv.cn

Py:   if not s:
来源：http://nfa.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hxw.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rth.xylfe.cn

TS:   if (s === "") {}
来源：http://kks.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://woq.bbcook.cn

Go:   if s == "" {}
来源：http://qiv.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://ehw.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vgi.tarul.cn

[E21] 超长截断加省略号
来源：http://qrv.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jxa.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zqz.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vic.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mlw.jinghuilouyu.cn


<!-- 参考信息 -->