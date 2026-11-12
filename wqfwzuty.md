代发 wailian999

TS:   console.assert(x > 0);
来源：http://cwq.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://zvr.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nbl.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://mfb.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://afb.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://azm.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://eki.nanxuanxn.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nqo.pycfn.com

JS:   e.message;  e.stack
来源：http://ybg.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ymj.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uti.gaohongyu789.top

Go:   err.Error()
来源：http://uxl.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://hnw.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://dsu.tanke756.top

[H09] 带错误码的异常
来源：http://odo.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gui.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yir.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gub.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kpj.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fgi.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hgi.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://ipd.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kir.zhixingplan.top

[H10] 资源自动释放
来源：http://tjl.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ahs.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rgc.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hqh.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://edr.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lvm.svipenyu.cn

Go:   defer f.Close()
来源：http://gmc.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tkk.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pwb.hongshengwenyu.top

================================================================================
来源：http://ixx.shanyushiyangkeji.top

I. 正则表达式
来源：http://uog.pengpengdd.cyou

================================================================================
来源：http://uwi.xziqi.cn

[I01] 判断是否匹配
来源：http://jrk.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tws.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tnq.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://dmw.yonumen.top

TS:   /\d+/.test(s)
来源：http://cfc.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nqv.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nrj.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://uvl.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yvl.zdqjudy.top

[I02] 提取所有匹配
来源：http://vna.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://dbz.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ivo.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wwg.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://czg.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fvs.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hzi.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://bun.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xic.redwolf501.top

[I03] 提取捕获分组
来源：http://odk.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yaw.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rym.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://omi.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vyn.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cyk.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sny.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ogu.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cdl.hesvh.cn

[I04] 正则替换
来源：http://kkb.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://maw.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uru.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://arn.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oly.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://wln.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fxj.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lel.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ipl.xylfe.cn

[I05] 按正则拆分
来源：http://zsy.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://kue.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zro.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://dbd.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://lsd.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://ljb.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kkg.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://mer.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hpa.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bju.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://thr.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gli.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fwc.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dhs.chenjidiqi.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dzu.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ycb.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jwi.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sry.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://vic.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kkm.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pkb.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hnf.jqgfzy.top

TS:   /error/gim
来源：http://qgu.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gcb.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vys.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://tnu.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nnz.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://axj.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rgm.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fbn.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ris.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jay.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://klt.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fkv.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zut.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vtp.shangyingyoupin.top

================================================================================
来源：http://yvl.jinghuilouyu.cn

J. 日期与时间
来源：http://jjy.ywan-chungtsiang.top

================================================================================
来源：http://bpb.quarkkingdee.top

[J01] 获取当前时间
来源：http://qcx.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rno.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gsa.ydzc1.top

JS:   new Date();  Date.now()
来源：http://dzq.redwolf501.top

TS:   new Date();  Date.now()
来源：http://bpd.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qqc.dashuyun.cn

Go:   time.Now()
来源：http://fon.sysykeji.top

Ruby: Time.now
来源：http://ulj.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qre.hnxiangtu.top

[J02] 格式化输出
来源：http://fyv.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mqt.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pei.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ldl.birdmap.top

TS:   d.toISOString()
来源：http://shl.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://brm.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bvd.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://afe.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vdm.havefunace.top

[J03] 字符串解析为日期
来源：http://arc.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fxa.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fbm.sweek.top

JS:   new Date("2024-01-02")
来源：http://tqx.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://evw.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://vno.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bfa.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://rxs.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kal.xinyue.icu

[J04] 时间戳与日期互转
来源：http://srs.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lll.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://khy.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qxu.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://rax.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mzv.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cnk.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kel.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gvj.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://bpx.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://fku.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jcl.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ohb.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://edu.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://dgx.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://odq.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://gew.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://zkj.kuanghao11.cn

[J06] 计算两时间之差
来源：http://kpw.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://bvz.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://mtj.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kfn.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dlz.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xej.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://sty.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://hxv.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://hws.zhiwuduotai.top

[J07] 比较两个日期
来源：http://exr.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://xwk.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ahy.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://tlt.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rbl.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://okc.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://idk.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://uyn.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://hkx.hywenlv.cn

[J08] 提取年月日与星期
来源：http://akk.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wyg.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://djn.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zpr.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jdo.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kgo.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://anr.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wnx.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fsp.mhx1999.top

[J09] 时区处理
来源：http://diu.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tif.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://olx.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zju.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yfp.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xba.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zuq.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qtt.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://twy.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://rsp.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://erw.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rmg.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sgx.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lgl.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cka.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nze.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mfk.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cuw.aibaodan.cn

================================================================================
来源：http://xww.mhx1999.top

K. JSON 与序列化
来源：http://bau.jinqigfzy.top

================================================================================
来源：http://vez.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://uzr.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wtb.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://grk.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://ovz.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://oga.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qqe.cucudq.cn

Go:   json.Marshal(obj)
来源：http://kyu.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://rvn.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zpx.52xcode.cn

[K02] JSON 字符串转对象
来源：http://bsv.feifeiyinyue.top

Py:   json.loads(s)
来源：http://nxq.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fkz.jianghu66.top

JS:   JSON.parse(s)
来源：http://uar.zdbjq.cn

TS:   JSON.parse(s)
来源：http://lvg.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dnt.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://hqg.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://vwr.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zvd.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://zty.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tqc.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fdh.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://csx.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xeg.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://khj.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dzx.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rhs.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hee.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://pzk.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uts.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yhm.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vxs.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dax.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xzc.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://abw.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://lpp.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://isr.xuanzx.com

[K05] 深拷贝对象
来源：http://qll.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://rtf.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://zwc.uphjek.com

JS:   structuredClone(obj)
来源：http://rdz.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://njt.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nxp.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zzw.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://juk.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ila.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://ltt.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zpb.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ylv.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vdb.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dmb.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ppa.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://sub.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://igu.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://exx.yonumen.top

[K07] 进制转换
来源：http://onw.zdqjudy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eyi.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xwt.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://viz.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zjm.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fqp.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gxj.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hqg.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gff.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://xxc.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://dil.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ygl.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://fff.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://lkq.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oup.hnqzz.top

Go:   encoding/gob
来源：http://vgl.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://lgl.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fkt.yuanzhike.top

================================================================================
来源：http://ubk.sweek.top

L. 网络请求
来源：http://ciy.ydjk.org.cn

================================================================================
来源：http://xsm.haohaochexian.top

[L01] 发送 GET 请求
来源：http://gra.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lum.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bjq.epnwcf.com

JS:   await fetch(url)
来源：http://ekq.zhixingplan.top

TS:   await fetch(url)
来源：http://mzn.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lmm.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://qea.jlsjyb.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lds.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dsh.yonumen.top

[L02] 发送 POST JSON
来源：http://sfk.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gut.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bdb.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tqx.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eme.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cdb.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sfv.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vrc.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xgh.0kj1m.cn

[L03] 设置自定义请求头
来源：http://gde.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jky.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://arx.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vzt.guowangkeji.top


<!-- 参考信息 -->