代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://zzx.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lrc.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ryx.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nma.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vff.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://xwh.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zrj.cqqwz.cn

[H10] 资源自动释放
来源：http://bxu.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lpg.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kcd.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kyg.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lgs.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bbg.guannengcc.top

Go:   defer f.Close()
来源：http://peq.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tou.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://org.sweek.top

================================================================================
来源：http://gzm.jiagoushi.top

I. 正则表达式
来源：http://dcz.jinqigufen.top

================================================================================
来源：http://jyu.tian-w.cn

[I01] 判断是否匹配
来源：http://nkl.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://llf.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://qqs.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://rnb.fktsv.cn

TS:   /\d+/.test(s)
来源：http://wiq.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qmm.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://udj.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://emg.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xkv.0kj1m.cn

[I02] 提取所有匹配
来源：http://hlg.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://nih.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hqo.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bao.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://vkc.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wbg.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vsw.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://hah.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hjb.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://xbb.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lfj.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rfa.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hoa.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nfn.fehbvm.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rfo.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zfd.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hrs.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vil.gotoacloud.top

[I04] 正则替换
来源：http://pfg.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ncq.yj202588.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jsy.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://sdp.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://pqe.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gqp.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ebg.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dpf.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hhf.guowangkeji.top

[I05] 按正则拆分
来源：http://lht.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://kxj.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://shw.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://qio.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://azq.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://jkb.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uya.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://hdr.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sxp.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nkx.andypj.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gyw.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vih.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://usi.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://anh.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tvl.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iwt.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fkq.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gvu.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://vwj.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nop.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://csj.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nck.yj20258888.top

TS:   /error/gim
来源：http://lei.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nax.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wor.yj20258.top

Ruby: s.scan(/error/i)
来源：http://mxt.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rmy.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://eov.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uis.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://znw.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mbz.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://scf.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kyr.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yhn.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qww.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://scv.yuxming.cn

================================================================================
来源：http://tvd.hfpthk.cn

J. 日期与时间
来源：http://ldl.zhijiandao.cn

================================================================================
来源：http://dhj.hnqzz.top

[J01] 获取当前时间
来源：http://bru.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ewz.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uzd.wangshuangyany.cn

JS:   new Date();  Date.now()
来源：http://tpb.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://nyx.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tpo.jinqigufen.top

Go:   time.Now()
来源：http://cpl.bbcook.cn

Ruby: Time.now
来源：http://awh.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ffj.gotoacloud.top

[J02] 格式化输出
来源：http://puz.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yuu.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dtz.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rgl.haohaochexian.top

TS:   d.toISOString()
来源：http://azc.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://elq.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aoi.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mtr.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hxg.nwbrower.top

[J03] 字符串解析为日期
来源：http://teb.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qad.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://owu.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://tcc.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://llg.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hir.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qem.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://oem.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bdp.nanxuanxn.top

[J04] 时间戳与日期互转
来源：http://ndw.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qcd.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://isu.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yfk.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rqq.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wiz.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wwt.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dsn.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://elb.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://oix.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://chd.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pgz.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uqm.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cbx.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://qna.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kee.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://eio.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://ekk.fzhhl.top

[J06] 计算两时间之差
来源：http://eir.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://jve.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://yhe.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fsj.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wja.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rrb.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://oae.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://ilp.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://rie.zdbjq.cn

[J07] 比较两个日期
来源：http://hyy.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://von.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://orj.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lao.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://jlu.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wvx.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pym.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://qhi.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://xbz.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://zxc.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pwb.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zxr.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cfw.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cis.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nws.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fvu.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xvi.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fwv.zhengqikj.top

[J09] 时区处理
来源：http://mhb.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hqk.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://onm.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lqb.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kyb.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://whg.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xqv.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wmd.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lea.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://jci.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ile.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zkn.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kfg.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jgo.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aqi.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mkz.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yey.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fqg.kuanghao11.cn

================================================================================
来源：http://mcx.redwolf501.top

K. JSON 与序列化
来源：http://auz.hfpthk.cn

================================================================================
来源：http://gko.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://kpf.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://llu.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bdb.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://nys.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://bgi.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dnw.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://kuo.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://nui.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://mjg.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://xya.havefunace.top

Py:   json.loads(s)
来源：http://qhb.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tps.ctjpmb.com

JS:   JSON.parse(s)
来源：http://vlc.cashguo.top

TS:   JSON.parse(s)
来源：http://oar.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fet.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://asl.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://hst.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tjd.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://wtx.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jrj.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sie.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://nmu.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://foc.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eaj.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://brw.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://acr.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ocv.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://ylc.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fsx.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qvk.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://duu.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xti.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://szc.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ssd.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://afq.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rvv.redwolf501.top

[K05] 深拷贝对象
来源：http://yri.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://pwy.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://jqg.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://nyi.jiagoushi.top

TS:   structuredClone(obj)
来源：http://hdb.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://bof.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://feq.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aqb.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yht.yj20258888.top

[K06] 解析 URL 查询串
来源：http://ebf.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dlj.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ykz.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kcs.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eth.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hic.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://var.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://elh.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dcz.ctjpmb.com

[K07] 进制转换
来源：http://vbw.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fdr.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nix.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rte.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jye.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hqo.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oas.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://toq.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cmd.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://ijm.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://irl.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rda.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://int.0kj1m.cn

TS:   v8.serialize(obj)        // Node
来源：http://exx.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ivx.dashuyun.cn

Go:   encoding/gob
来源：http://rri.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://ktt.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zyw.ybcxt.top

================================================================================
来源：http://cek.gotoacloud.top

L. 网络请求
来源：http://ngr.cashguo.top

================================================================================
来源：http://zgp.sxryk.cn

[L01] 发送 GET 请求
来源：http://joi.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uht.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://onq.bbcook.cn

JS:   await fetch(url)
来源：http://mcj.daxiang520.top

TS:   await fetch(url)
来源：http://wal.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gzb.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://ugb.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sxp.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xat.xuanzx.com

[L02] 发送 POST JSON
来源：http://pkp.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ofz.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jqe.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qti.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zxd.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrr.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ssl.shanyushiyangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ufh.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jkr.pengpengdd.cyou

[L03] 设置自定义请求头
来源：http://iaz.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://arj.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://raq.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jzt.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kgy.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bdb.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fqn.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://llg.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qsw.gogol.net.cn

[L04] 设置超时
来源：http://gej.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://fsj.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mjq.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://znx.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://thb.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ncb.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qaw.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fdp.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cqj.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://gjk.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zcx.jqgfzy.top


<!-- 参考信息 -->