代发 wailian999

[D15] 去重
来源：http://jth.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nvt.bbcook.cn

PHP:  array_unique($arr);
来源：http://gkb.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://fkc.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://qkt.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zlv.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://jnz.yvedp.cn

Ruby: arr.uniq
来源：http://cpx.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://fuf.zhijiandao.cn

[D16] 求和与平均值
来源：http://xok.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mrq.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wry.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zym.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dad.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dto.vehdjk.com

Go:   // 手写循环累加
来源：http://qvk.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uyk.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://lqs.52xcode.cn

[D17] 最大值与最小值
来源：http://lvx.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://kjc.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://yql.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vbj.yuanzhike.top

TS:   Math.max(...arr);
来源：http://tqq.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nre.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fyb.ivvv.top

Ruby: arr.max;  arr.min
来源：http://blu.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://ezq.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://ytv.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hqg.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://let.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ubi.jinghuilouyu.cn

TS:   nested.flat();
来源：http://adk.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dpz.cheryme.top

Go:   // 手写双层循环
来源：http://fge.gotoacloud.top

Ruby: nested.flatten
来源：http://ajz.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xod.jqgufenzy.top

[D19] 按字段分组
来源：http://efh.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pug.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tqj.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gme.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hbt.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fcu.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://xyw.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fxp.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yce.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://zje.shuidangran.top

Py:   Counter(arr)
来源：http://mrw.yueranfly.top

PHP:  array_count_values($arr);
来源：http://cai.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxr.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oav.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://msz.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://uad.gotoacloud.top

Ruby: arr.tally
来源：http://jvw.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yem.bjfxy.top

[D21] 判断是否包含某元素
来源：http://atd.ybcxt.top

Py:   x in arr
来源：http://chn.yuanzhike.top

PHP:  in_array($x, $arr, true);
来源：http://eql.guannengcc.top

JS:   arr.includes(x)
来源：http://gzw.gogol.net.cn

TS:   arr.includes(x)
来源：http://aus.sysykeji.top

Java: list.contains(x)
来源：http://htu.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://iec.yj20258888.top

Ruby: arr.include?(x)
来源：http://nqt.hywenlv.cn

C#:   list.Contains(x)
来源：http://ymy.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://qsx.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yza.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qfa.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zkp.zdqjudy.top

TS:   [...arr];
来源：http://shx.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://tuk.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://nqd.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://sfw.bjfxy.top

C#:   new List<int>(list);
来源：http://ujd.ydjk.org.cn

[D23] reduce 累积计算
来源：http://wrr.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kpn.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vqc.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hre.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xcn.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sat.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://keb.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lii.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jrt.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://uxv.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mca.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qot.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jqg.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jad.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qnm.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lxo.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vro.cheryme.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://igh.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://etd.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mee.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rqq.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nqa.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eex.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tfy.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fcn.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://flt.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dqe.hysaishi.cn

[D26] 数组转字符串
来源：http://bpg.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://vqb.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://bad.sxryk.cn

JS:   arr.join(", ")
来源：http://jia.cqqwz.cn

TS:   arr.join(", ")
来源：http://pgz.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://itd.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://cjb.chenlongwang.top

Ruby: arr.join(", ")
来源：http://eks.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://ycg.ybcxt.top

================================================================================
来源：http://kxj.redwolf501.top

E. 字符串处理
来源：http://tkr.dashuyun.cn

================================================================================
来源：http://rfv.hywenlv.cn

[E01] 拼接字符串
来源：http://onk.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rtt.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pyu.haohaochexian.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zfx.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://plm.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rrb.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lem.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uvv.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nge.vqdsnc.cn

[E02] 重复字符串
来源：http://lxu.nanxuanxn.top

Py:   "ab" * 3
来源：http://xez.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://foo.fktsv.cn

JS:   "ab".repeat(3)
来源：http://fia.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://jjg.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://flj.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://uyz.fzhhl.top

Ruby: "ab" * 3
来源：http://guj.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tsy.hongshengwenyu.top

[E03] 截取子串
来源：http://xyf.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cwm.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tsf.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bew.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://zyj.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://naz.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mtd.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://jco.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://qfe.aizwys.cn

[E04] 查找子串位置
来源：http://iik.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://ccl.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://hfu.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dcb.ydzc1.top

TS:   s.indexOf("x")
来源：http://jkl.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://vrn.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://akx.jinqigfzy.top

Ruby: s.index("x")
来源：http://owu.bjfxy.top

C#:   s.IndexOf("x")
来源：http://dib.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hzc.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cvx.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pqz.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lwe.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ems.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pjm.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://znb.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zaf.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kko.xinyue.icu

[E06] 替换子串
来源：http://brz.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vak.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://sfu.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vbe.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://vee.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vqr.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xdc.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ypf.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://xzm.andypj.xyz

[E07] 按分隔符拆分
来源：http://ybw.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fxs.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ysr.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uwe.wangdashe.top

TS:   s.split(",")
来源：http://oje.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://lkj.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lbh.tarul.cn

Ruby: s.split(",");  s.split
来源：http://cdz.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xtw.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://bsu.tarul.cn

Py:   ",".join(items)
来源：http://muf.hammf.cn

PHP:  implode(",", $items);
来源：http://biz.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://kmd.nanxinkj.top

TS:   items.join(",")
来源：http://vxe.jlsjyb.cn

Java: String.join(",", items)
来源：http://plo.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://pmp.hywenlv.cn

Ruby: items.join(",")
来源：http://wvm.jinqigufen.top

C#:   string.Join(",", items)
来源：http://ydu.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://nau.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://flk.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hss.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://fhf.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://nbk.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://gnn.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fbu.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bkz.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cbv.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://fku.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qmd.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://euq.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://eox.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://rei.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://lhu.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xdj.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fsy.zhaomingkeji.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://erw.mhx1999.top

[E11] 反转字符串
来源：http://ifm.zhoulong.xyz

Py:   s[::-1]
来源：http://cio.snrcjt.cn

PHP:  strrev($s);
来源：http://rcs.cashguo.top

JS:   [...s].reverse().join("")
来源：http://hix.yj202588.top

TS:   [...s].reverse().join("")
来源：http://nfi.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zys.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lub.uphjek.com

Ruby: s.reverse
来源：http://nac.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://obh.sweek.top

[E12] 统计某字符出现次数
来源：http://lfz.yuanzhike.top

Py:   s.count("a")
来源：http://gvw.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://jwu.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://ilz.jianghu66.top

TS:   s.split("a").length - 1
来源：http://fpp.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://osx.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://bdc.nanxinkj.top

Ruby: s.count("a")
来源：http://yro.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://pyb.yanxiufei.cn

[E13] 逐字符遍历
来源：http://wyz.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://pil.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qhz.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://idf.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kax.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fxc.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ykw.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mxc.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fxl.yj20258888.top

[E14] URL 编码与 Base64
来源：http://yny.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ola.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lfs.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hrz.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gnx.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uxm.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lrs.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hyt.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bmy.gogol.net.cn

[E15] HTML 转义 / 反转义
来源：http://cvb.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mlf.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://llb.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wll.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hyg.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ckh.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gge.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aez.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kja.xylfe.cn

[E16] 数字千分位
来源：http://wek.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://fbs.jqgfzy.top

PHP:  number_format(1234567);
来源：http://kbe.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://jjm.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jhc.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wrf.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ovh.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ycv.cheryme.top

C#:   1234567.ToString("N0")
来源：http://ktx.shzxlz.cn

[E17] 首字母大写
来源：http://fml.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://joi.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ucn.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yjs.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ihl.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oqq.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fgq.jiagoushi.top

Ruby: s.capitalize
来源：http://jmj.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://end.hcnkem.com

[E18] 模板占位符替换
来源：http://xka.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://feb.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sfx.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rlx.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ism.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uac.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yjd.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fei.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eas.52xcode.cn

[E19] 多行文本按行拆分
来源：http://fim.wangdashe.top

Py:   s.splitlines()
来源：http://qyf.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zrp.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://rwn.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://rpf.52xcode.cn

Java: s.lines().toList()
来源：http://kfk.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://zbx.zhaomingkeji.xyz

Ruby: s.lines
来源：http://dsa.316326.xyz

C#:   s.Split('\n')
来源：http://drv.yongpay.top

[E20] 判断字符串是否为空
来源：http://kzq.shangyingyoupin.top

Py:   if not s:
来源：http://adg.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uih.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xyn.wangdashe.top

TS:   if (s === "") {}
来源：http://hwh.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://lzc.yuxming.cn

Go:   if s == "" {}
来源：http://grn.chenjidiqi.icu

Ruby: if s.empty?
来源：http://ekc.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://swu.uphjek.com

[E21] 超长截断加省略号
来源：http://fwo.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mtq.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ukx.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vfy.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qdj.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uhu.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://pjl.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vul.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eds.ydzc1.top


<!-- 参考信息 -->