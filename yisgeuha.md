代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nmx.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://jim.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://pks.uphjek.com

[H10] 资源自动释放
来源：http://hbx.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kyt.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eaf.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nxg.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qsq.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fsz.xziqi.cn

Go:   defer f.Close()
来源：http://yrb.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cdw.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wdf.iojbl.cn

================================================================================
来源：http://rkj.fktsv.cn

I. 正则表达式
来源：http://mbb.zycfv.cn

================================================================================
来源：http://kcc.zhixingplan.top

[I01] 判断是否匹配
来源：http://xvy.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jwu.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://pyw.pycfn.com

JS:   /\d+/.test(s)
来源：http://lfr.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://ajx.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tdm.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hpu.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://fzz.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dib.cucudq.cn

[I02] 提取所有匹配
来源：http://vfr.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://ymx.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vxw.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pwj.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://csv.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tog.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://irm.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://gmc.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://isp.yuxming.cn

[I03] 提取捕获分组
来源：http://kip.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ltu.jiagoushi.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qub.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cqy.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vue.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zju.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nrm.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zyv.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tdh.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://vcq.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pwk.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wli.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lnp.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://ovt.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fzo.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://umu.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wec.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ghd.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://mhe.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ujm.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tah.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://muq.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://sqj.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://hdz.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dfl.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ofa.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rrx.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://afc.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ydb.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hhd.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ogq.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zqp.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://moq.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://snz.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hsu.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://meu.tanke756.top

[I07] 忽略大小写与多行模式
来源：http://qih.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eyc.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nnd.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zch.jqgfzy.top

TS:   /error/gim
来源：http://hvk.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oic.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qys.pycfn.com

Ruby: s.scan(/error/i)
来源：http://fkx.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ozn.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://zll.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mee.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dvv.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ppv.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bqz.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ohq.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bwd.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zak.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mvj.chenjidiqi.icu

================================================================================
来源：http://rtc.sufxvd.cn

J. 日期与时间
来源：http://ues.hnqzz.top

================================================================================
来源：http://thu.sjlbkw.cn

[J01] 获取当前时间
来源：http://qzi.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fjn.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yga.uphjek.com

JS:   new Date();  Date.now()
来源：http://tfw.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://ijt.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ind.quarkkingdee.top

Go:   time.Now()
来源：http://ant.daria6918.cn

Ruby: Time.now
来源：http://abf.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://roq.vqdsnc.cn

[J02] 格式化输出
来源：http://syk.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bnv.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://auy.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tww.redwolf501.top

TS:   d.toISOString()
来源：http://wgi.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hcs.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vhc.zhaomingkeji.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txz.zdbjq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xjv.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://zbk.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rcj.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nzk.daxiang520.top

JS:   new Date("2024-01-02")
来源：http://nho.meibo888.top

TS:   new Date("2024-01-02")
来源：http://bez.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://evr.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eno.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://dty.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ojp.sysykeji.top

[J04] 时间戳与日期互转
来源：http://mba.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kkf.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hou.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uru.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rfh.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nox.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lsi.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bze.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://awg.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://auf.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://ols.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qld.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltm.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bnc.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://tdm.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rjy.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://tcl.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://kaf.yuxming.cn

[J06] 计算两时间之差
来源：http://edi.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://sjj.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://gxj.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sdb.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mkl.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ydq.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://qab.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://uov.hywenlv.cn

C#:   (end - start).TotalSeconds
来源：http://fpm.hywenlv.cn

[J07] 比较两个日期
来源：http://ihy.redwolf501.top

Py:   d1 < d2;  d1 == d2
来源：http://rfk.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://brl.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://emj.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://xix.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qih.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tlq.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://hjg.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://kjw.fzhhl.top

[J08] 提取年月日与星期
来源：http://gpd.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ldc.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ywy.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vtv.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ucc.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://psf.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://arf.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://huh.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hjy.uphjek.com

[J09] 时区处理
来源：http://dww.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kgh.gotoacloud.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zxs.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jii.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kuv.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fwj.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ltq.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mug.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mfu.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://hlr.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://zez.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yps.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bpe.redwolf501.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://juk.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://biz.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bsb.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rzm.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kce.cdnleiting.top

================================================================================
来源：http://xoe.hammf.cn

K. JSON 与序列化
来源：http://mvu.gogol.net.cn

================================================================================
来源：http://iyx.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://ujd.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xkj.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://asg.cashguo.top

JS:   JSON.stringify(obj)
来源：http://own.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://jxh.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nyv.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://hrm.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://nlp.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://toj.yj20258888.top

[K02] JSON 字符串转对象
来源：http://oxb.aibaodan.cn

Py:   json.loads(s)
来源：http://ngc.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hzu.yueranfly.top

JS:   JSON.parse(s)
来源：http://puk.svipenyu.cn

TS:   JSON.parse(s)
来源：http://yhm.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://faz.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://rup.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://dob.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vtc.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://ofe.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zdf.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qpy.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://cjf.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lcc.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jxz.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ckp.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tmn.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pxv.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://ylq.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sxi.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xtf.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rhm.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxi.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qjy.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hpl.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://itr.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kdo.epnwcf.com

[K05] 深拷贝对象
来源：http://ggb.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://tah.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://dba.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://ijr.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://qul.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bdq.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wax.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ste.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dgf.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://xxa.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://clt.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jzv.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tcv.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tva.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://feq.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://alw.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://stn.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kst.yuxming.cn

[K07] 进制转换
来源：http://tmi.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tow.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lub.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qle.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wcl.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vsj.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wer.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kmd.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mdb.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://czt.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://aow.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yhq.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://jvn.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://bpg.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sae.mhx1999.top

Go:   encoding/gob
来源：http://nxb.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://wph.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iyb.sysykeji.top

================================================================================
来源：http://ncs.jinqigfzy.top

L. 网络请求
来源：http://fbe.fengsongda.top

================================================================================
来源：http://tqw.hcnkem.com

[L01] 发送 GET 请求
来源：http://irj.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mpb.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xya.meibo888.top

JS:   await fetch(url)
来源：http://qsn.meibo888.top

TS:   await fetch(url)
来源：http://brl.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://udl.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://llz.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ibg.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hls.daria6918.cn

[L02] 发送 POST JSON
来源：http://wwk.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bkm.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dyu.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rdf.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mxp.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kww.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://slr.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pba.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ypn.yangfankeji.com

[L03] 设置自定义请求头
来源：http://tds.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sck.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nxk.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gab.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nmc.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oyu.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://msx.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ebx.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bfr.aibaodan.cn

[L04] 设置超时
来源：http://key.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://rtd.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hup.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vec.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pkt.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mpk.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mux.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://npf.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ajs.fzhhl.top

[L05] 上传文件（multipart）
来源：http://vhj.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xsd.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kyg.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://caq.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kaq.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wda.xuanzx.com


<!-- 参考信息 -->