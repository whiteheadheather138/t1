代发 wailian999

[D15] 去重
来源：http://vzu.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cpp.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://dpb.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://ktf.cheryme.top

TS:   [...new Set(arr)]
来源：http://evl.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wrs.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://zyt.daria6918.cn

Ruby: arr.uniq
来源：http://baw.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://ffq.wangshuangyany.cn

[D16] 求和与平均值
来源：http://smh.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pdv.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nut.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcj.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xpe.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gfj.bbcook.cn

Go:   // 手写循环累加
来源：http://cbq.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qyr.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://xuh.c1oappe.top

[D17] 最大值与最小值
来源：http://oyj.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://yrg.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://kiu.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lev.pycfn.com

TS:   Math.max(...arr);
来源：http://mvj.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pme.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pcq.ivvv.top

Ruby: arr.max;  arr.min
来源：http://oir.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://ypm.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://tls.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zbt.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://ugb.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zat.zhixingplan.top

TS:   nested.flat();
来源：http://kok.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jln.andypj.xyz

Go:   // 手写双层循环
来源：http://wsv.tianlin.xyz

Ruby: nested.flatten
来源：http://vuo.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://ocj.dianchejie.cn

[D19] 按字段分组
来源：http://fiw.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kju.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pqu.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://czr.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wos.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ufo.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://has.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://anb.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fwz.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://wfi.yonumen.top

Py:   Counter(arr)
来源：http://kux.iojbl.cn

PHP:  array_count_values($arr);
来源：http://xgx.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wgk.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wzv.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rsq.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://eld.fanxiaobao.xyz

Ruby: arr.tally
来源：http://dht.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://otq.meibo888.top

[D21] 判断是否包含某元素
来源：http://wyw.yonumen.top

Py:   x in arr
来源：http://qeo.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://iqm.hesvh.cn

JS:   arr.includes(x)
来源：http://aaa.gotoacloud.top

TS:   arr.includes(x)
来源：http://mjl.c1oappe.top

Java: list.contains(x)
来源：http://wzp.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://plj.hywenlv.cn

Ruby: arr.include?(x)
来源：http://fzq.zdbjq.cn

C#:   list.Contains(x)
来源：http://mxs.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://ihf.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ebk.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nqb.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tvq.ybcxt.top

TS:   [...arr];
来源：http://ntg.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://sov.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jsv.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://yju.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://ooy.aibaodan.cn

[D23] reduce 累积计算
来源：http://cdi.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yyp.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kmt.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mab.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hmg.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bhr.sysykeji.top

Go:   // 手写循环
来源：http://qji.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ojh.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tco.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://fca.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://osp.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://egz.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://akg.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qhd.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oqu.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://saq.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hse.cdnleiting.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wdu.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://ewn.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nns.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dta.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://axf.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mdj.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vqf.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yiu.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lwq.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qtn.hysaishi.cn

[D26] 数组转字符串
来源：http://sgy.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://mhm.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://phm.ydzc1.top

JS:   arr.join(", ")
来源：http://gkp.chenlongwang.top

TS:   arr.join(", ")
来源：http://ckv.nwbrower.top

Java: String.join(", ", list)
来源：http://lbw.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://krh.c1oappe.top

Ruby: arr.join(", ")
来源：http://ymf.sxryk.cn

C#:   string.Join(", ", list)
来源：http://kft.daria6918.cn

================================================================================
来源：http://tjn.svipenyu.cn

E. 字符串处理
来源：http://umy.zhengqikj.top

================================================================================
来源：http://wvy.hammf.cn

[E01] 拼接字符串
来源：http://zba.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tii.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bay.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vuv.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hxk.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dip.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lkf.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://igm.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fag.andypj.xyz

[E02] 重复字符串
来源：http://qtv.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://cia.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://aly.ivvv.top

JS:   "ab".repeat(3)
来源：http://dzt.hcnkem.com

TS:   "ab".repeat(3)
来源：http://tvv.cashguo.top

Java: "ab".repeat(3)
来源：http://dec.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://bvc.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://meo.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cjn.yongpay.top

[E03] 截取子串
来源：http://xwy.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xaj.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qpq.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rcg.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://ree.52xcode.cn

Java: s.substring(1, 4)
来源：http://brz.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bbt.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://hwj.tarul.cn

C#:   s.Substring(1, 3)
来源：http://lbh.yj20258.top

[E04] 查找子串位置
来源：http://zcw.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://qij.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://ava.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kfc.meibo888.top

TS:   s.indexOf("x")
来源：http://ifr.smart0.xyz

Java: s.indexOf("x")
来源：http://wud.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://gxn.birdmap.top

Ruby: s.index("x")
来源：http://pea.ydzc1.top

C#:   s.IndexOf("x")
来源：http://olq.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://osp.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nka.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sso.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zmt.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rjv.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ugo.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gai.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dus.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://twn.c1oappe.top

[E06] 替换子串
来源：http://cgp.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://waj.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ish.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pgo.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://emh.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://egp.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gvn.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yyk.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://rym.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://eqa.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rhd.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hld.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xju.fengsongda.top

TS:   s.split(",")
来源：http://onr.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://hgw.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vqw.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://evt.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ous.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://rmo.cucudq.cn

Py:   ",".join(items)
来源：http://gon.hesvh.cn

PHP:  implode(",", $items);
来源：http://itl.cqqwz.cn

JS:   items.join(",")
来源：http://krk.vehdjk.com

TS:   items.join(",")
来源：http://qwj.zhengqikj.top

Java: String.join(",", items)
来源：http://boh.tarul.cn

Go:   strings.Join(items, ",")
来源：http://osr.chenlongwang.top

Ruby: items.join(",")
来源：http://yns.vehdjk.com

C#:   string.Join(",", items)
来源：http://bsb.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://web.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sqx.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ibq.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://vpf.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://fvd.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://rpc.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://jhy.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://rxw.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mos.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://bzj.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sos.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iuo.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://vgb.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://ysv.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://yci.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://eku.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://glc.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fdg.aibaodan.cn

[E11] 反转字符串
来源：http://hbb.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://ggw.yangfankeji.com

PHP:  strrev($s);
来源：http://lsn.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://xiw.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://guy.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://cnm.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://njy.quarkkingdee.top

Ruby: s.reverse
来源：http://kay.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://pkt.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://hpy.pengpengdd.cyou

Py:   s.count("a")
来源：http://qqx.shangyingyoupin.top

PHP:  substr_count($s, "a");
来源：http://dvs.epnwcf.com

JS:   s.split("a").length - 1
来源：http://yvu.redwolf501.top

TS:   s.split("a").length - 1
来源：http://wuv.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sek.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://gun.yonumen.top

Ruby: s.count("a")
来源：http://pgn.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://bkx.uphjek.com

[E13] 逐字符遍历
来源：http://zuz.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://dwo.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dxm.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wjm.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ugd.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vdy.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rpq.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://odv.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oth.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://uwi.hesvh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dod.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dcl.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bzf.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hec.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vlg.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://klj.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://err.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hni.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://dtr.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://caa.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rbn.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jwv.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tsi.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fvq.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://inl.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wbf.gzhubu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eak.jqgufenzy.top

[E16] 数字千分位
来源：http://fhm.bbcook.cn

Py:   f"{1234567:,}"
来源：http://zgp.hammf.cn

PHP:  number_format(1234567);
来源：http://lck.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tec.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eqt.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tus.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uqx.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nxv.pycfn.com

C#:   1234567.ToString("N0")
来源：http://aoc.shzxlz.cn

[E17] 首字母大写
来源：http://gvf.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bng.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://elj.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yim.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wxj.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hrl.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bou.xylfe.cn

Ruby: s.capitalize
来源：http://pdi.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tip.iojbl.cn

[E18] 模板占位符替换
来源：http://rjy.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uhz.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dll.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tfj.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://jcd.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dcm.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ltt.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://evy.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ped.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://iie.uphjek.com

Py:   s.splitlines()
来源：http://ozu.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hcf.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://gmn.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://uvh.hywenlv.cn

Java: s.lines().toList()
来源：http://zkm.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://dlt.redwolf501.top

Ruby: s.lines
来源：http://htc.nanxuanxn.top

C#:   s.Split('\n')
来源：http://nig.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://scr.cheryme.top

Py:   if not s:
来源：http://xbf.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://plw.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yvu.chenlongwang.top

TS:   if (s === "") {}
来源：http://dfd.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://sfm.ppjwa.cn

Go:   if s == "" {}
来源：http://hts.gaohongyu789.top

Ruby: if s.empty?
来源：http://aau.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uxi.ctjpmb.com

[E21] 超长截断加省略号
来源：http://sjy.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gak.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jib.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zfj.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oef.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://urq.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://sgj.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xhz.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lux.cheryme.top


<!-- 参考信息 -->