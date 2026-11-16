代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yby.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://cwk.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ljw.daxiang520.top

[H10] 资源自动释放
来源：http://hdi.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eze.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wbj.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vkz.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cts.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fhb.zhijiandao.cn

Go:   defer f.Close()
来源：http://mfz.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cgr.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oes.yvedp.cn

================================================================================
来源：http://jqk.zdbjq.cn

I. 正则表达式
来源：http://hbb.iojbl.cn

================================================================================
来源：http://kxa.guannengcc.top

[I01] 判断是否匹配
来源：http://gut.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ffh.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vqe.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://ptq.yj20258.top

TS:   /\d+/.test(s)
来源：http://you.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vta.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cqn.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://dph.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dzc.zhongyouzk.top

[I02] 提取所有匹配
来源：http://ats.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://qsq.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ert.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ymh.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://hga.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://epq.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kgc.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://pll.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mym.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://htm.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://roj.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ykk.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cnq.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oni.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dmg.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ozr.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vfh.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://unq.cashguo.top

[I04] 正则替换
来源：http://gzi.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yem.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pyb.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://era.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://egv.ybcxt.top

Java: s.replaceAll("\\d+", "#")
来源：http://fmo.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lzt.jinyuanbaomall.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eec.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kia.birdmap.top

[I05] 按正则拆分
来源：http://poj.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sxj.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jbq.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://zjm.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://olq.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://olu.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hrx.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gzm.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fdy.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mve.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://owq.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rja.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mhr.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ctf.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://phb.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ccm.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vlb.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://net.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://mkd.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jzw.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ehl.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://juu.dianchejie.cn

TS:   /error/gim
来源：http://owh.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ffg.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lgu.yongpay.top

Ruby: s.scan(/error/i)
来源：http://dup.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vzh.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://yck.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://syb.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://irw.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ncw.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bzs.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sea.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jmm.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gif.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zxf.zdbjq.cn

================================================================================
来源：http://ulb.ywan-chungtsiang.top

J. 日期与时间
来源：http://evn.svipenyu.cn

================================================================================
来源：http://izc.xylfe.cn

[J01] 获取当前时间
来源：http://pgf.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mpi.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bkn.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://ecm.andypj.xyz

TS:   new Date();  Date.now()
来源：http://qsy.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fce.zhoulong.xyz

Go:   time.Now()
来源：http://mcr.xuetiantiany.cn

Ruby: Time.now
来源：http://ezd.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mjj.meibo888.top

[J02] 格式化输出
来源：http://vyc.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://agz.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cfm.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kqe.zycfv.cn

TS:   d.toISOString()
来源：http://uxg.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jih.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lvx.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wne.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rdk.cqqwz.cn

[J03] 字符串解析为日期
来源：http://zug.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yvv.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iir.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://tzd.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://lcb.jqgufenzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://xcg.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ylz.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://neo.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bil.mhx1999.top

[J04] 时间戳与日期互转
来源：http://thw.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tia.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://flx.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rjr.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rwr.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lgx.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rmp.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xxq.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ccm.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://mbm.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://yjx.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bgw.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rqe.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jln.iojbl.cn

Java: LocalDate.now().plusDays(7)
来源：http://btk.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ift.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://vwo.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jol.yueranfly.top

[J06] 计算两时间之差
来源：http://hoc.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://fsf.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://cxx.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gky.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sxg.tarul.cn

Java: Duration.between(start, end).toSeconds()
来源：http://khg.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://jbb.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://yfr.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://ebw.jlsjyb.cn

[J07] 比较两个日期
来源：http://zwj.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://lpr.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xvq.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://gty.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://mwa.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://emi.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lgh.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://ift.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://rni.jqgfzy.top

[J08] 提取年月日与星期
来源：http://ycb.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cio.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pzu.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rrv.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ctu.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lio.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://apm.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dcp.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nmw.iojbl.cn

[J09] 时区处理
来源：http://zin.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jvf.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tfr.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dtu.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vit.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pfn.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vvd.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://msq.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://weh.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://qzm.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nse.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vbk.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qcm.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hwi.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mbt.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wna.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ovs.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rpu.zycfv.cn

================================================================================
来源：http://doh.c1oappe.top

K. JSON 与序列化
来源：http://pui.yanxiufei.cn

================================================================================
来源：http://cwl.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://pmw.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xpr.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vlx.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://qeu.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://sri.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ryq.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://ypx.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://otw.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tpk.yonumen.top

[K02] JSON 字符串转对象
来源：http://ipw.quarkkingdee.top

Py:   json.loads(s)
来源：http://aiw.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cdt.fehbvm.com

JS:   JSON.parse(s)
来源：http://fug.yonumen.top

TS:   JSON.parse(s)
来源：http://wrb.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dfw.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://jzi.jianghu66.top

Ruby: JSON.parse(s)
来源：http://ljo.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vid.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://tau.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pui.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ysh.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pkc.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ipd.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dlc.zhongyouzk.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vql.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://kyz.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rnn.gzhubu.top

[K04] 读取 JSON 文件
来源：http://sym.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bbz.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ahj.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wqp.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://smp.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://orf.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pua.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eqw.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tpg.yuxming.cn

[K05] 深拷贝对象
来源：http://xkd.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://fay.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://zmr.snrcjt.cn

JS:   structuredClone(obj)
来源：http://lfk.xziqi.cn

TS:   structuredClone(obj)
来源：http://xgr.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bfu.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rmb.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pek.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://smn.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://glp.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jte.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://amy.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zoj.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ujp.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://saq.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://neq.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ljs.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hiy.316326.xyz

[K07] 进制转换
来源：http://sib.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lle.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fsf.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vob.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uzp.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wxh.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ipq.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qeh.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xjs.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://swa.yj202588.top

Py:   pickle.dumps(obj)
来源：http://hal.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fyn.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://wxk.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://gsr.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://evq.xziqi.cn

Go:   encoding/gob
来源：http://htf.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://vti.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xmj.fanxiaobao.xyz

================================================================================
来源：http://ror.uphjek.com

L. 网络请求
来源：http://rxo.xuetiantiany.cn

================================================================================
来源：http://hye.haohaochexian.top

[L01] 发送 GET 请求
来源：http://jrt.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vva.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kqm.uphjek.com

JS:   await fetch(url)
来源：http://lsp.epnwcf.com

TS:   await fetch(url)
来源：http://yrz.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kgr.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://edf.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bgj.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mgw.ivvv.top

[L02] 发送 POST JSON
来源：http://pye.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://miw.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yzi.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vav.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nlv.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nqa.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ezi.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dqo.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fzj.52xcode.cn

[L03] 设置自定义请求头
来源：http://wzh.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yeq.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tqw.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gqc.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eyp.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nda.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qrv.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jun.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zkq.shanyushiyangkeji.top

[L04] 设置超时
来源：http://men.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://jwm.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fmj.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ibl.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxo.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vvv.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rxg.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://weh.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xpi.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://ssi.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lil.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wgw.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bbk.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hxv.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://viy.snrcjt.cn


<!-- 参考信息 -->