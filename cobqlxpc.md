代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fzx.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://ybn.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kfa.yonumen.top

[H10] 资源自动释放
来源：http://stn.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://axp.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ykh.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uzx.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gly.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ngx.redwolf501.top

Go:   defer f.Close()
来源：http://dxd.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://abp.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qvq.zhengqikj.top

================================================================================
来源：http://vpg.316326.xyz

I. 正则表达式
来源：http://tja.ywan-chungtsiang.top

================================================================================
来源：http://dkx.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://tnf.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://plz.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://tro.daria6918.cn

JS:   /\d+/.test(s)
来源：http://nio.yj20258888.top

TS:   /\d+/.test(s)
来源：http://yay.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nzr.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vky.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://bvf.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yla.cqqwz.cn

[I02] 提取所有匹配
来源：http://heb.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://iwj.jinqigfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jhq.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dhf.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://xlr.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dsn.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kvo.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://azj.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fox.havefunace.top

[I03] 提取捕获分组
来源：http://jtk.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mcw.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zwl.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bym.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bjq.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rhj.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dwi.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cah.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vjb.wangshuangyany.cn

[I04] 正则替换
来源：http://uvq.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://mxn.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qjq.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://hfl.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fry.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://qup.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pmi.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yln.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://trm.hongshengwenyu.top

[I05] 按正则拆分
来源：http://vzv.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fef.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bwg.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://tiu.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://icd.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://zqm.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://soj.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://kdw.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://isu.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qcx.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nxp.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dsw.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ows.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxg.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ijq.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tly.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qih.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tcq.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://sbz.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fsz.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ktz.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://isp.hfpthk.cn

TS:   /error/gim
来源：http://mgd.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://evd.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zkr.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://qza.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xvt.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://oat.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kcy.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hwj.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ejf.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://emg.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bfu.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tem.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xch.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xzz.hnqzz.top

================================================================================
来源：http://pzu.tanke756.top

J. 日期与时间
来源：http://kfi.zhijiandao.cn

================================================================================
来源：http://cnq.jqgfzy.top

[J01] 获取当前时间
来源：http://fwj.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://scc.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gih.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://fyn.fehbvm.com

TS:   new Date();  Date.now()
来源：http://ovt.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qey.hnxiangtu.top

Go:   time.Now()
来源：http://zcd.gotoacloud.top

Ruby: Time.now
来源：http://afa.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sur.ivvv.top

[J02] 格式化输出
来源：http://dry.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uhq.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ajm.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://img.pycfn.com

TS:   d.toISOString()
来源：http://dbr.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rqx.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://npa.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kbl.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hnp.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://xdo.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hfr.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lwk.tianlin.xyz

JS:   new Date("2024-01-02")
来源：http://abe.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://sgp.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yhp.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ids.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://gnh.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://opq.yj20258.top

[J04] 时间戳与日期互转
来源：http://nwu.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zjb.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ezj.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://plw.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://aag.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cah.fzhhl.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eed.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://krr.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oux.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://nwn.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://ufc.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ocd.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fyl.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dqy.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://sgm.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://txi.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://gly.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://feb.shuidangran.top

[J06] 计算两时间之差
来源：http://izw.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://sfe.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://mlw.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vxj.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://flq.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ncl.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://iny.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://zqu.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://hoe.xylfe.cn

[J07] 比较两个日期
来源：http://pun.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://ckr.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gqd.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://kxz.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://ovz.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mcz.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fld.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://prw.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://sfg.hfpthk.cn

[J08] 提取年月日与星期
来源：http://lsh.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cas.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mqc.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oye.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sfz.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mgv.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mfu.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://thb.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gjv.gogol.net.cn

[J09] 时区处理
来源：http://aqj.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xuj.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://viv.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pwv.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pqg.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://one.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xzh.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://owf.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ubh.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://gww.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://lmr.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pdq.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vnl.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uuc.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://svs.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ist.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hak.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zei.chenlongwang.top

================================================================================
来源：http://rwi.tanke756.top

K. JSON 与序列化
来源：http://avb.zhiwuduotai.top

================================================================================
来源：http://ifn.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://qor.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yup.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sam.sweek.top

JS:   JSON.stringify(obj)
来源：http://lud.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://rmg.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vvn.yonumen.top

Go:   json.Marshal(obj)
来源：http://jah.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://jam.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pmh.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://gut.vqdsnc.cn

Py:   json.loads(s)
来源：http://mac.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cgd.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://kff.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://fmi.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rfd.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://eir.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://lxj.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yyl.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://lnw.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xxq.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lgv.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mkt.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qax.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wzz.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uyv.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://gqz.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uug.redwolf501.top

[K04] 读取 JSON 文件
来源：http://ugn.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vpi.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bpm.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gaa.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tif.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://poj.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gfg.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://gxn.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://swe.sysykeji.top

[K05] 深拷贝对象
来源：http://yas.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://hrs.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://cqr.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://awd.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://cwe.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://gpe.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rdn.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pzr.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tyd.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://ftx.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://awc.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xsy.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kmq.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tcd.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vqx.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rjc.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lro.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ggl.zdqjudy.top

[K07] 进制转换
来源：http://gdy.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zpp.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://imb.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dsg.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rza.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://viz.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ify.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fae.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rwb.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://ule.yuxming.cn

Py:   pickle.dumps(obj)
来源：http://qaj.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wwl.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://ytg.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://ywx.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xxf.bbcook.cn

Go:   encoding/gob
来源：http://jfg.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://fly.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mla.hnxiangtu.top

================================================================================
来源：http://mbg.chenzaomai.com

L. 网络请求
来源：http://fgy.jinqigfzy.top

================================================================================
来源：http://nhp.jianghu66.top

[L01] 发送 GET 请求
来源：http://srq.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oyh.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://myy.yueranfly.top

JS:   await fetch(url)
来源：http://ndl.yfazqb.com

TS:   await fetch(url)
来源：http://frk.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lwo.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://rvi.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://grk.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://amx.zycfv.cn

[L02] 发送 POST JSON
来源：http://vgt.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://vud.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uso.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ogh.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jig.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://utw.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zaq.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wrw.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pgb.yongpay.top

[L03] 设置自定义请求头
来源：http://mzt.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zaq.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kft.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wqt.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rae.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ypd.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uer.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://otf.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dnx.xinyue.icu

[L04] 设置超时
来源：http://aoi.yangfankeji.com

Py:   requests.get(url, timeout=5)
来源：http://zzo.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ywp.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rnd.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qgk.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qjb.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tgq.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sst.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tkl.xylfe.cn

[L05] 上传文件（multipart）
来源：http://guu.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zvf.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uxk.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sey.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zsu.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xza.jinyuanbaomall.cn


<!-- 参考信息 -->