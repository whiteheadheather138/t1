代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://szf.pycfn.com

Go:   // 手写循环
来源：http://gdj.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bip.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uhw.vehdjk.com

[D15] 去重
来源：http://kky.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lyh.daria6918.cn

PHP:  array_unique($arr);
来源：http://tmw.gzhubu.top

JS:   [...new Set(arr)]
来源：http://rlc.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://xsk.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fbu.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dnp.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://aep.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://frs.xylfe.cn

[D16] 求和与平均值
来源：http://hok.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fjq.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cck.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xly.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cmk.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vah.snrcjt.cn

Go:   // 手写循环累加
来源：http://vjk.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rhd.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://cvr.svipenyu.cn

[D17] 最大值与最小值
来源：http://rmq.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://ocp.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://cdq.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tcf.zhengqikj.top

TS:   Math.max(...arr);
来源：http://ywj.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://moh.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oip.ybcxt.top

Ruby: arr.max;  arr.min
来源：http://dow.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://vfa.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://eva.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lsa.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://myz.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gbe.xuanzx.com

TS:   nested.flat();
来源：http://ytp.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bud.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://eou.yuanzhike.top

Ruby: nested.flatten
来源：http://trr.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eue.quarkkingdee.top

[D19] 按字段分组
来源：http://ufb.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jzo.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iad.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ajr.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aao.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wkj.yj202588.top

Go:   // 手写 map[string][]T
来源：http://hkw.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mjq.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zka.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://klz.hnxiangtu.top

Py:   Counter(arr)
来源：http://usy.zycfv.cn

PHP:  array_count_values($arr);
来源：http://qjo.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wuo.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hzi.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://juu.cheryme.top

Go:   // 手写 map[T]int
来源：http://kaa.c1oappe.top

Ruby: arr.tally
来源：http://wdg.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nko.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://bfm.yongpay.top

Py:   x in arr
来源：http://fpu.yuanzhike.top

PHP:  in_array($x, $arr, true);
来源：http://fxy.uphjek.com

JS:   arr.includes(x)
来源：http://jab.cdnleiting.top

TS:   arr.includes(x)
来源：http://smg.guowangkeji.top

Java: list.contains(x)
来源：http://itz.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://ivy.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://lrz.meibo888.top

C#:   list.Contains(x)
来源：http://bgw.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://kna.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://abq.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://law.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rub.shzxlz.cn

TS:   [...arr];
来源：http://bxf.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://oen.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://wox.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://bhr.yj20258888.top

C#:   new List<int>(list);
来源：http://ppv.fengsongda.top

[D23] reduce 累积计算
来源：http://eyr.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qwl.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mou.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jwo.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ksb.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://srr.havefunace.top

Go:   // 手写循环
来源：http://owk.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://puu.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ptp.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://his.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wtr.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fph.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ahj.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vim.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xti.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wck.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gmj.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qou.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://toq.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://voh.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://atd.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lyb.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wto.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jru.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ved.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eeo.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://esi.xuanzx.com

[D26] 数组转字符串
来源：http://sql.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://nxr.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://sju.zhaomingkeji.xyz

JS:   arr.join(", ")
来源：http://xus.0kj1m.cn

TS:   arr.join(", ")
来源：http://qqn.316326.xyz

Java: String.join(", ", list)
来源：http://zmq.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://yez.xziqi.cn

Ruby: arr.join(", ")
来源：http://gah.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://jms.mhx1999.top

================================================================================
来源：http://vre.pengpengdd.cyou

E. 字符串处理
来源：http://jog.pengpengdd.cyou

================================================================================
来源：http://omw.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://yuo.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tno.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kki.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vbj.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qgs.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pud.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uwi.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://add.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://red.hammf.cn

[E02] 重复字符串
来源：http://zdm.jqgfzy.top

Py:   "ab" * 3
来源：http://kkq.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://xos.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://jwa.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://npx.jinqigufen.top

Java: "ab".repeat(3)
来源：http://bwn.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://wpb.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://zjn.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ffa.fengsongda.top

[E03] 截取子串
来源：http://zhk.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rvo.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vjd.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bcy.xinyue.icu

TS:   s.slice(1, 4)
来源：http://lsf.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://pyd.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aqj.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://zyh.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://mnl.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://gwc.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://lrs.daria6918.cn

PHP:  strpos($s, "x");
来源：http://jxe.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ohw.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://mya.bbcook.cn

Java: s.indexOf("x")
来源：http://xau.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://ruz.hysaishi.cn

Ruby: s.index("x")
来源：http://cav.epnwcf.com

C#:   s.IndexOf("x")
来源：http://zmu.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gnk.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hzb.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pav.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vqo.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wam.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gep.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hog.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aka.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bbd.tianlin.xyz

[E06] 替换子串
来源：http://tba.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nyr.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://vxq.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nbq.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://gjr.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jov.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lia.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fip.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://kib.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://zsb.haohaochexian.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dww.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://avc.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://oxh.zdbjq.cn

TS:   s.split(",")
来源：http://wqg.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://apf.xinyue.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lxz.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://urc.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pzf.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://san.iojbl.cn

Py:   ",".join(items)
来源：http://jgr.guowangkeji.top

PHP:  implode(",", $items);
来源：http://bun.haohaochexian.top

JS:   items.join(",")
来源：http://oue.aizwys.cn

TS:   items.join(",")
来源：http://rqz.tanke756.top

Java: String.join(",", items)
来源：http://lnj.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://nxn.wangshuangyany.cn

Ruby: items.join(",")
来源：http://xkh.gotoacloud.top

C#:   string.Join(",", items)
来源：http://tre.yvedp.cn

[E09] 去除所有空白字符
来源：http://jyu.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tam.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nzo.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://pcw.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://nqz.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://yhl.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dch.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://klw.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lcj.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://ysl.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ffc.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lhu.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://gwa.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://chg.vehdjk.com

Java: String.format("%03d", 7)
来源：http://qfr.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hob.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ykm.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lfi.daria6918.cn

[E11] 反转字符串
来源：http://hqa.pycfn.com

Py:   s[::-1]
来源：http://pyj.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://czo.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://thm.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://qce.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mll.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yee.gotoacloud.top

Ruby: s.reverse
来源：http://vtg.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://mvg.guannengcc.top

[E12] 统计某字符出现次数
来源：http://tgh.sysykeji.top

Py:   s.count("a")
来源：http://slb.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://ope.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://tzc.yangfankeji.com

TS:   s.split("a").length - 1
来源：http://wyd.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tzd.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://vqj.yonumen.top

Ruby: s.count("a")
来源：http://znv.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://imj.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://iin.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://soy.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cwb.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://duv.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://swn.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xbq.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pzk.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://emv.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://whs.cucudq.cn

[E14] URL 编码与 Base64
来源：http://ctk.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zxq.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://nfl.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ffm.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sfi.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wef.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rav.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hlc.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://anv.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://umg.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uxh.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wqc.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jwu.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hhv.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yll.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sig.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://azo.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tky.shzxlz.cn

[E16] 数字千分位
来源：http://kus.tian-w.cn

Py:   f"{1234567:,}"
来源：http://gwp.cheryme.top

PHP:  number_format(1234567);
来源：http://opm.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ayd.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gcn.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pzi.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ggk.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aaw.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://bhg.aibaodan.cn

[E17] 首字母大写
来源：http://djv.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://exz.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://eqy.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xbw.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://czy.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://inb.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jpf.dashuyun.cn

Ruby: s.capitalize
来源：http://jxm.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://std.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://bwc.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cwn.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://unw.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lff.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kvf.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ndc.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://voh.yuanzhike.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bay.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zus.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://ggr.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://izi.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://axa.xingfuxueyuan.xyz

JS:   s.split(/\r?\n/)
来源：http://kdh.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://eeq.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://rux.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://gzy.yj20258888.top

Ruby: s.lines
来源：http://wbt.sjlbkw.cn

C#:   s.Split('\n')
来源：http://oho.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://fxg.cqqwz.cn

Py:   if not s:
来源：http://tkk.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nfa.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yxf.daxiang520.top

TS:   if (s === "") {}
来源：http://lyn.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://aqq.quarkkingdee.top

Go:   if s == "" {}
来源：http://quw.aibaodan.cn

Ruby: if s.empty?
来源：http://rxg.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jcm.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://yxy.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ztv.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hqq.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://avr.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xmh.jqgfzy.top


<!-- 参考信息 -->