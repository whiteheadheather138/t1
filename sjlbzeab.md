代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://nko.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bqw.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xjg.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ykh.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rsp.ydzc1.top

Go:   defer f.Close()
来源：http://qad.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hej.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cnm.zhongyouzk.top

================================================================================
来源：http://weo.sxryk.cn

I. 正则表达式
来源：http://ngd.c1oappe.top

================================================================================
来源：http://xje.redwolf501.top

[I01] 判断是否匹配
来源：http://sgr.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ali.ehwqpu.com

PHP:  preg_match('/\d+/', $s);
来源：http://vna.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://krk.cheryme.top

TS:   /\d+/.test(s)
来源：http://jqt.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bzg.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kuq.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://qcc.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oqe.meibo888.top

[I02] 提取所有匹配
来源：http://nek.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://alo.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xof.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xhq.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://tzk.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://riq.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mww.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://xes.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kji.mhx1999.top

[I03] 提取捕获分组
来源：http://mbi.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://grg.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zyn.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iyx.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vkm.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dxy.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aez.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://njd.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sff.yj20258888.top

[I04] 正则替换
来源：http://lyz.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://npl.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://raf.aizwys.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lyu.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://use.aibaodan.cn

Java: s.replaceAll("\\d+", "#")
来源：http://auz.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gix.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://pym.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rsp.shuidangran.top

[I05] 按正则拆分
来源：http://zfb.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://slv.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pdj.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://ofr.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://odb.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://uuc.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bjg.jinghuilouyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xnt.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blb.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lhx.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eyi.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ipg.yangfankeji.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cjc.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tid.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ibk.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qzd.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dgt.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ohi.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://tdq.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tfn.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mwb.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xgd.tian-w.cn

TS:   /error/gim
来源：http://mtm.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xen.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xyf.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://fce.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hqo.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://axy.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://keo.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dic.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ytk.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hap.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rhz.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cqd.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mwh.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zvo.jyoumei.cn

================================================================================
来源：http://bdy.316326.xyz

J. 日期与时间
来源：http://gtd.smart0.xyz

================================================================================
来源：http://fgi.haohaochexian.top

[J01] 获取当前时间
来源：http://ukw.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://thn.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nof.aizwys.cn

JS:   new Date();  Date.now()
来源：http://ybw.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://jhx.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pra.sxryk.cn

Go:   time.Now()
来源：http://sfg.wangdashe.top

Ruby: Time.now
来源：http://unt.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://occ.mhx1999.top

[J02] 格式化输出
来源：http://hwa.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iuv.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://knd.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hsh.cqqwz.cn

TS:   d.toISOString()
来源：http://nsx.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://znm.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pet.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gvr.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mpc.gogol.net.cn

[J03] 字符串解析为日期
来源：http://boq.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nqu.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hec.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://yja.cashguo.top

TS:   new Date("2024-01-02")
来源：http://tui.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jik.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hcq.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://kyl.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://krm.meibo888.top

[J04] 时间戳与日期互转
来源：http://jjo.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xjl.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aut.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ink.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kbu.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qrs.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wux.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bpe.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wpp.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://paq.havefunace.top

Py:   now + timedelta(days=7)
来源：http://tvp.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://elt.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ffq.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oqw.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://aki.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xpy.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://zgx.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tlg.birdmap.top

[J06] 计算两时间之差
来源：http://qdz.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://qoo.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://nja.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zox.cqqwz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wfh.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://esc.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://paf.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://hti.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://dlt.dashuyun.cn

[J07] 比较两个日期
来源：http://pxt.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://vhj.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ldc.ybcxt.top

JS:   d1.getTime() < d2.getTime()
来源：http://dxi.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://sao.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vyd.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pbq.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://ohv.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://txx.gotoacloud.top

[J08] 提取年月日与星期
来源：http://dlw.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://drn.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dgi.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pzq.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fur.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uwj.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fpo.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bdv.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cte.hnxiangtu.top

[J09] 时区处理
来源：http://rlm.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pgi.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://opo.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gnw.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lwt.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kzt.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ume.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ujh.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zes.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://uhl.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://buy.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tls.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bcq.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qpb.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gnw.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nuw.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://udm.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hjw.zhijiandao.cn

================================================================================
来源：http://ydk.sysykeji.top

K. JSON 与序列化
来源：http://byz.sjlbkw.cn

================================================================================
来源：http://ebu.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://cyd.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gez.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dou.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://jsx.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://tsj.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tso.cashguo.top

Go:   json.Marshal(obj)
来源：http://yan.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://uve.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dhv.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://azy.uphjek.com

Py:   json.loads(s)
来源：http://rxn.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://flr.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://tbl.haohaochexian.top

TS:   JSON.parse(s)
来源：http://qyq.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jzk.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://hmw.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://yec.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fec.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://uej.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://afd.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vpk.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jpx.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ujv.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pqt.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mef.hesvh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ewv.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qpu.cashguo.top

[K04] 读取 JSON 文件
来源：http://czj.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aag.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rdb.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tmx.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sch.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bjc.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://abl.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zje.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vzx.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://nfe.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://vmm.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://hkm.tianlin.xyz

JS:   structuredClone(obj)
来源：http://atb.vehdjk.com

TS:   structuredClone(obj)
来源：http://ppt.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lsg.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vjm.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://enu.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jyp.shuidangran.top

[K06] 解析 URL 查询串
来源：http://mvd.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jqj.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hdj.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gle.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggt.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gzj.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bil.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://onl.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lvq.ppjwa.cn

[K07] 进制转换
来源：http://mzf.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pqe.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wns.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ktk.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eqh.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pwj.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ihj.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kkh.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yih.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://ptp.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://fhm.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jxl.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://iyu.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://qfb.shuidangran.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gdn.fzhhl.top

Go:   encoding/gob
来源：http://bdo.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://kfj.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ook.yj20258.top

================================================================================
来源：http://izf.aibaodan.cn

L. 网络请求
来源：http://bdv.nanxinkj.top

================================================================================
来源：http://zag.dashuyun.cn

[L01] 发送 GET 请求
来源：http://myl.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zag.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wxx.yongpay.top

JS:   await fetch(url)
来源：http://ltz.yuanzhike.top

TS:   await fetch(url)
来源：http://nnm.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iuo.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://vkv.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rqy.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yrv.ydzc1.top

[L02] 发送 POST JSON
来源：http://wxm.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://spc.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bgk.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vbo.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yoa.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qcu.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eex.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ugj.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ryt.yfazqb.com

[L03] 设置自定义请求头
来源：http://znb.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iea.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://akk.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://slv.xuanzx.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xwv.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zkf.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jva.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bey.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://efi.shanyushiyangkeji.top

[L04] 设置超时
来源：http://emb.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://grh.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yvy.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cdt.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ipg.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wvn.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ccn.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fyg.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ond.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://pgs.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nmh.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mtc.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xqi.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mxb.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ovh.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nzu.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cjp.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hcr.zycfv.cn

[L06] 解析响应为 JSON
来源：http://pse.xuanzx.com


<!-- 参考信息 -->