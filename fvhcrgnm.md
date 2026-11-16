代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://jew.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vcl.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tyh.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uwb.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rjq.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://knt.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ifh.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jws.pycfn.com

================================================================================
来源：http://msy.ydjk.org.cn

I. 正则表达式
来源：http://wyx.hnxiangtu.top

================================================================================
来源：http://upm.dianchejie.cn

[I01] 判断是否匹配
来源：http://ott.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rog.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vlp.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://yko.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://umu.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lpu.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xbs.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://cxh.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pxm.bbcook.cn

[I02] 提取所有匹配
来源：http://fng.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://dys.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cfk.yvedp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wvb.cheryme.top

TS:   s.match(/\d+/g)
来源：http://aaz.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mmi.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aun.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://wyr.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qpp.redwolf501.top

[I03] 提取捕获分组
来源：http://zip.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hjm.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eqk.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hgo.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ixj.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hsk.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kkk.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rud.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vgg.shangyingyoupin.top

[I04] 正则替换
来源：http://bkk.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bxp.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wbk.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://abm.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://ccx.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://iqn.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://owh.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://owj.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hxo.gzhubu.top

[I05] 按正则拆分
来源：http://pqb.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cun.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rep.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://ipl.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://bdy.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://nrf.hywenlv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rmr.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://byz.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://imw.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lvt.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ubp.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iee.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hmk.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zka.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dtn.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vla.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nal.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://srl.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://qcr.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ezd.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hre.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zag.gzhubu.top

TS:   /error/gim
来源：http://nta.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://toc.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qbj.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://mdz.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wue.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://qch.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ekv.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vpk.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vvo.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://avx.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uas.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gfk.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blk.kuanghao11.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bqe.dashuyun.cn

================================================================================
来源：http://qqb.andypj.xyz

J. 日期与时间
来源：http://oqh.tanke756.top

================================================================================
来源：http://yuc.chenlongwang.top

[J01] 获取当前时间
来源：http://xgr.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rcq.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sue.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://gbc.mhx1999.top

TS:   new Date();  Date.now()
来源：http://exu.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://czi.52xcode.cn

Go:   time.Now()
来源：http://szg.ivvv.top

Ruby: Time.now
来源：http://lmy.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sby.gogol.net.cn

[J02] 格式化输出
来源：http://ghf.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uju.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ggo.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mlv.fzhhl.top

TS:   d.toISOString()
来源：http://jmy.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ngo.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vcp.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nan.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hqf.daxiang520.top

[J03] 字符串解析为日期
来源：http://dry.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nzk.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jru.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://qjc.xuetiantiany.cn

TS:   new Date("2024-01-02")
来源：http://qks.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uua.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wvy.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://pjy.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://szr.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://skx.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uqv.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sca.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vsy.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://bci.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ash.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rfi.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gqb.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oae.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://kbt.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://kkz.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ooq.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qoi.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zvy.iojbl.cn

Java: LocalDate.now().plusDays(7)
来源：http://vak.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xbd.hfpthk.cn

Ruby: Time.now + 7 * 86400
来源：http://wlr.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://plo.shzxlz.cn

[J06] 计算两时间之差
来源：http://pub.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://kbv.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://eco.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://frk.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kco.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ziw.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://vnq.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://yno.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://fcl.tianlin.xyz

[J07] 比较两个日期
来源：http://ezd.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://jik.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tsb.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jod.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xyx.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://thj.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dio.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://ajl.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://sun.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://ghv.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lsi.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fql.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qev.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ryf.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hmf.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oui.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://beh.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rcc.chenlongwang.top

[J09] 时区处理
来源：http://dam.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qdd.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yni.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ryn.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sux.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ekw.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://goa.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vks.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qav.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://tqr.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://cja.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tzn.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gtx.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://znl.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hir.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://quh.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qdk.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zko.zhaomingkeji.xyz

================================================================================
来源：http://ouo.cucudq.cn

K. JSON 与序列化
来源：http://kun.aibaodan.cn

================================================================================
来源：http://mdr.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://hkj.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wdk.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ylq.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://vba.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://ydj.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pmp.fktsv.cn

Go:   json.Marshal(obj)
来源：http://aqf.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://apc.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://jsi.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://bmo.aibaodan.cn

Py:   json.loads(s)
来源：http://mwl.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bxg.xuanzx.com

JS:   JSON.parse(s)
来源：http://bce.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://nst.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cta.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://srd.iojbl.cn

Ruby: JSON.parse(s)
来源：http://omm.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sky.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://kim.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pce.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qiw.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qpv.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://isq.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ktk.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lbl.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://ald.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://heb.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://xyg.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cxs.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ptj.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eos.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vcd.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xuc.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mzv.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fjt.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dio.ppjwa.cn

[K05] 深拷贝对象
来源：http://caa.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://tym.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://oia.bbcook.cn

JS:   structuredClone(obj)
来源：http://fqb.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://lfk.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ero.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pvc.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jjq.kuanghao11.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mlv.xylfe.cn

[K06] 解析 URL 查询串
来源：http://egs.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oaq.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dbi.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fye.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yvl.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jxq.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tba.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://voa.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://acq.guowangkeji.top

[K07] 进制转换
来源：http://hpd.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qfz.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mpv.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rjl.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bce.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vjv.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sjr.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hpz.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aec.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://ixr.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://bbp.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yyn.yanxiufei.cn

JS:   v8.serialize(obj)        // Node
来源：http://tqb.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://nkw.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rsq.guannengcc.top

Go:   encoding/gob
来源：http://kop.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://gks.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uod.gotoacloud.top

================================================================================
来源：http://trp.redwolf501.top

L. 网络请求
来源：http://bqk.zdbjq.cn

================================================================================
来源：http://pce.yvedp.cn

[L01] 发送 GET 请求
来源：http://hdz.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wfl.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uhb.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://jjt.316326.xyz

TS:   await fetch(url)
来源：http://lay.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ohj.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://akn.ctjpmb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xyi.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gjc.tianlin.xyz

[L02] 发送 POST JSON
来源：http://khx.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qyc.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dbt.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://drr.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fra.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rzl.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xbd.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lbo.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xdc.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://wwh.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xkg.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ulk.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ufu.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zrf.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baj.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vqs.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nuq.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vgk.guannengcc.top

[L04] 设置超时
来源：http://nfn.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://wku.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rbw.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gbc.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xsj.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fag.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ngb.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rjd.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qxr.yj20258888.top

[L05] 上传文件（multipart）
来源：http://etp.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dkv.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://naz.dianchejie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ztq.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zeg.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nrx.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sbw.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aqb.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qkm.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://dww.iojbl.cn


<!-- 参考信息 -->