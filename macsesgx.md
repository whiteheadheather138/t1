代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://uba.cheryme.top

Go:   // 手写循环
来源：http://ssw.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://itl.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dby.yj202588.top

[D15] 去重
来源：http://kan.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ggs.ctjpmb.com

PHP:  array_unique($arr);
来源：http://smh.hammf.cn

JS:   [...new Set(arr)]
来源：http://fbi.ydzc1.top

TS:   [...new Set(arr)]
来源：http://ufu.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ryi.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pyt.cucudq.cn

Ruby: arr.uniq
来源：http://tdb.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://jnv.xziqi.cn

[D16] 求和与平均值
来源：http://rgz.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dcn.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zjm.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sso.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://maz.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://muj.cucudq.cn

Go:   // 手写循环累加
来源：http://fbn.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zqx.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://xdb.snrcjt.cn

[D17] 最大值与最小值
来源：http://fyu.yonumen.top

Py:   max(arr);  min(arr)
来源：http://vsw.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://mcq.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rjw.sxryk.cn

TS:   Math.max(...arr);
来源：http://fxp.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iqo.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nwu.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://ofr.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://vvl.cashguo.top

[D18] 扁平化嵌套数组
来源：http://ego.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uwh.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://avr.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zsd.tarul.cn

TS:   nested.flat();
来源：http://dhf.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eqr.yanxiufei.cn

Go:   // 手写双层循环
来源：http://zef.feifeiyinyue.top

Ruby: nested.flatten
来源：http://wqb.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://wje.quarkkingdee.top

[D19] 按字段分组
来源：http://lnb.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://akj.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xtl.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dhu.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://nwz.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ddp.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://syx.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://utd.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rcb.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://pvq.hfpthk.cn

Py:   Counter(arr)
来源：http://ybw.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://rsr.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fvu.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kam.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://knf.havefunace.top

Go:   // 手写 map[T]int
来源：http://wrg.316326.xyz

Ruby: arr.tally
来源：http://qxm.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sfb.iojbl.cn

[D21] 判断是否包含某元素
来源：http://vlk.yj20258.top

Py:   x in arr
来源：http://udb.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://bkv.52xcode.cn

JS:   arr.includes(x)
来源：http://rpd.shzxlz.cn

TS:   arr.includes(x)
来源：http://odq.meibo888.top

Java: list.contains(x)
来源：http://mow.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://kph.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://jau.yuanzhike.top

C#:   list.Contains(x)
来源：http://gqa.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://alk.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kwf.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://upa.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://knx.shangyingyoupin.top

TS:   [...arr];
来源：http://exi.tanke756.top

Java: new ArrayList<>(list);
来源：http://ory.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zhs.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://hln.ehwqpu.com

C#:   new List<int>(list);
来源：http://jwn.jlsjyb.cn

[D23] reduce 累积计算
来源：http://rlj.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vxk.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pyj.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qgk.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rwg.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yce.zhoulong.xyz

Go:   // 手写循环
来源：http://mtb.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ole.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jyj.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://zkd.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mqk.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xcf.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hht.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hkr.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rqr.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yeu.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bsi.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pyt.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://gxh.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ehk.yanxiufei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zsh.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kte.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qmb.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cxy.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dxo.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xdy.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rmj.cdnleiting.top

[D26] 数组转字符串
来源：http://zkl.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://urv.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://tpp.gotoacloud.top

JS:   arr.join(", ")
来源：http://xpl.fengsongda.top

TS:   arr.join(", ")
来源：http://geq.c1oappe.top

Java: String.join(", ", list)
来源：http://glr.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://cvu.tanke756.top

Ruby: arr.join(", ")
来源：http://oow.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://gqx.yonumen.top

================================================================================
来源：http://igo.guowangkeji.top

E. 字符串处理
来源：http://dis.cqqwz.cn

================================================================================
来源：http://rxj.ybcxt.top

[E01] 拼接字符串
来源：http://mlu.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pdx.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://exq.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ymw.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jjr.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aph.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yha.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://drj.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fki.zdqjudy.top

[E02] 重复字符串
来源：http://vcx.aibaodan.cn

Py:   "ab" * 3
来源：http://kwk.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://nrm.nwbrower.top

JS:   "ab".repeat(3)
来源：http://qku.tarul.cn

TS:   "ab".repeat(3)
来源：http://lro.gotoacloud.top

Java: "ab".repeat(3)
来源：http://cag.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://bss.xziqi.cn

Ruby: "ab" * 3
来源：http://ltu.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qtp.yuanzhike.top

[E03] 截取子串
来源：http://ghy.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hkg.yj20258888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://emj.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ldg.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://hwi.andypj.xyz

Java: s.substring(1, 4)
来源：http://yvw.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fbz.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://rxx.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://zyz.yvedp.cn

[E04] 查找子串位置
来源：http://gjo.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://ruu.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://uvw.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cjh.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://krb.tarul.cn

Java: s.indexOf("x")
来源：http://nab.havefunace.top

Go:   strings.Index(s, "x")
来源：http://zlu.epnwcf.com

Ruby: s.index("x")
来源：http://roz.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://kiy.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zmc.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://guz.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eag.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kfu.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rvm.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ntd.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iyh.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://axh.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fkl.guannengcc.top

[E06] 替换子串
来源：http://jui.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vef.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://dvl.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zgb.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://gvi.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://txb.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wyi.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://goa.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://hob.gogol.net.cn

[E07] 按分隔符拆分
来源：http://hsk.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wqj.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hap.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tjn.shanyushiyangtech.top

TS:   s.split(",")
来源：http://duv.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kqh.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rvt.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://nhk.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://env.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://tyh.aizwys.cn

Py:   ",".join(items)
来源：http://njw.tianlin.xyz

PHP:  implode(",", $items);
来源：http://hoi.daxiang520.top

JS:   items.join(",")
来源：http://fzo.yj202588.top

TS:   items.join(",")
来源：http://jzy.daxiang520.top

Java: String.join(",", items)
来源：http://shd.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://ztj.yj20258.top

Ruby: items.join(",")
来源：http://gyd.svipenyu.cn

C#:   string.Join(",", items)
来源：http://vcy.vehdjk.com

[E09] 去除所有空白字符
来源：http://jct.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lbq.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nfe.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://phc.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ffh.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://evw.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://art.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kyy.cqqwz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mdw.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://bzb.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://veg.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hba.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://rev.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://qef.epnwcf.com

Java: String.format("%03d", 7)
来源：http://fim.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fei.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vrt.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wzi.jlsjyb.cn

[E11] 反转字符串
来源：http://anw.ybcxt.top

Py:   s[::-1]
来源：http://xwk.fzhhl.top

PHP:  strrev($s);
来源：http://vfp.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://twq.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://juu.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wyk.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://iuy.sysykeji.top

Ruby: s.reverse
来源：http://buf.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dfe.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://bgd.fehbvm.com

Py:   s.count("a")
来源：http://chg.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://giw.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://fbo.hesvh.cn

TS:   s.split("a").length - 1
来源：http://sjp.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tcr.316326.xyz

Go:   strings.Count(s, "a")
来源：http://tje.daxiang520.top

Ruby: s.count("a")
来源：http://vig.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://fnc.hysaishi.cn

[E13] 逐字符遍历
来源：http://gcq.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://equ.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gwn.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ngw.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tsy.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vyx.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hkk.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://cvx.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fht.wangdashe.top

[E14] URL 编码与 Base64
来源：http://fqe.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nja.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://glg.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jwh.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vik.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tix.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jet.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sct.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nqs.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://daa.epnwcf.com

Py:   html.escape(s);  html.unescape(s)
来源：http://pyl.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xna.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://azh.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://qir.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bec.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lpl.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vao.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xbn.havefunace.top

[E16] 数字千分位
来源：http://kse.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://bep.yangfankeji.com

PHP:  number_format(1234567);
来源：http://gsw.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://orh.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vbl.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cqr.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gar.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://muw.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://dyz.dianchejie.cn

[E17] 首字母大写
来源：http://lti.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gkz.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gih.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eml.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fbo.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxy.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mko.redwolf501.top

Ruby: s.capitalize
来源：http://rxv.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sxd.mhx1999.top

[E18] 模板占位符替换
来源：http://nmg.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aoi.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rqr.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uoe.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://twc.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yja.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qwa.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mof.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sij.yfazqb.com

[E19] 多行文本按行拆分
来源：http://alc.haohaochexian.top

Py:   s.splitlines()
来源：http://aru.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ghs.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://apx.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://gqz.ctjpmb.com

Java: s.lines().toList()
来源：http://tbx.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://kav.ehwqpu.com

Ruby: s.lines
来源：http://vqy.hnxiangtu.top

C#:   s.Split('\n')
来源：http://fkk.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://odo.tanke756.top

Py:   if not s:
来源：http://itz.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wjk.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hgb.ybcxt.top

TS:   if (s === "") {}
来源：http://jfd.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://gkx.jinqigufen.top

Go:   if s == "" {}
来源：http://wlt.chenjidiqi.icu

Ruby: if s.empty?
来源：http://noy.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nqa.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://zhf.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zuo.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://raz.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aqb.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://amu.yj20258888.top


<!-- 参考信息 -->