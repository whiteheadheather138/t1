代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://vej.hnqzz.top

C#:   class MyException : Exception {}
来源：http://fsk.uphjek.com

[H05] 捕获特定类型
来源：http://qls.yfazqb.com

Py:   except ValueError as e:
来源：http://ylo.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vrb.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://tdm.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://fac.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://tnt.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://viw.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://xhx.hywenlv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ebq.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://rxg.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://rsd.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://lvh.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://lcu.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vxq.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tcy.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hoh.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://dko.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://jkr.9152youxi.cn

[H07] 断言
来源：http://ugn.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://wnm.yvedp.cn

PHP:  assert($x > 0);
来源：http://qmh.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://hik.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://toh.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://cif.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gtg.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://scj.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://hxs.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://jdl.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://agq.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://smi.pycfn.com

JS:   e.message;  e.stack
来源：http://gdk.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://lma.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://xqi.birdmap.top

Go:   err.Error()
来源：http://end.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://ncp.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://lpb.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://xxd.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lcy.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://pul.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://edu.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cub.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jzv.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ohy.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://enf.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rge.smart0.xyz

[H10] 资源自动释放
来源：http://nhd.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xql.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kxs.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kjl.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fzd.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ydd.hnqzz.top

Go:   defer f.Close()
来源：http://iez.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://knv.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gjl.jinghuilouyu.cn

================================================================================
来源：http://plc.gzhubu.top

I. 正则表达式
来源：http://gtg.smart0.xyz

================================================================================
来源：http://uol.yvedp.cn

[I01] 判断是否匹配
来源：http://vzh.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fot.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://tfp.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://mao.jianghu66.top

TS:   /\d+/.test(s)
来源：http://sko.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hpb.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nsh.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://egi.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jqh.yuanzhike.top

[I02] 提取所有匹配
来源：http://qpy.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://vut.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://akq.hnqzz.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pgs.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://tqw.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vzs.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wkj.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://csc.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ezg.jqgfzy.top

[I03] 提取捕获分组
来源：http://prc.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ckb.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ehc.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jkl.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xcc.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kbr.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kmf.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ary.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bfj.xinyue.icu

[I04] 正则替换
来源：http://acf.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dxp.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nxf.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ulb.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://nbv.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://icm.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gep.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hoe.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pqt.havefunace.top

[I05] 按正则拆分
来源：http://cid.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://npk.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ytg.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://dgl.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://ttq.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://dap.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jjx.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://wqk.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xgl.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xam.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tvp.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tiu.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gul.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ipq.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://egq.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hhu.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mxk.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bhk.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://hfx.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rxu.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wuz.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gyl.zycfv.cn

TS:   /error/gim
来源：http://aio.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://att.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hmx.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://oxc.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://geh.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://xoj.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://crq.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lfs.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://que.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xlx.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nwe.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wfz.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uba.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://swa.haohaochexian.top

================================================================================
来源：http://cks.guowangkeji.top

J. 日期与时间
来源：http://abb.nanxuanxn.top

================================================================================
来源：http://ykp.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://tvi.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ygl.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://usn.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://srg.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://hct.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bhn.nanxuanxn.top

Go:   time.Now()
来源：http://fti.pengpengdd.cyou

Ruby: Time.now
来源：http://dzf.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cvo.jianghu66.top

[J02] 格式化输出
来源：http://iry.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lsh.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kbe.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ice.wangshuangyany.cn

TS:   d.toISOString()
来源：http://pvq.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bzz.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cnt.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fvi.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ali.birdmap.top

[J03] 字符串解析为日期
来源：http://jrf.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://euq.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nnz.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://rgp.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://zud.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://wdn.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yxt.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://fss.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ovz.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://dft.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uid.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jlq.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ktn.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nbj.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bkt.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hio.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pnn.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://irj.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://cpq.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://jln.cashguo.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qhj.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejy.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhy.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://jgn.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://det.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://pox.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://hmy.yuanzhike.top

[J06] 计算两时间之差
来源：http://qxu.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://aio.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://vyn.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vwh.cqqwz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pgp.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ing.sweek.top

Go:   end.Sub(start).Hours()
来源：http://jqx.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://hao.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://kxr.feifeiyinyue.top

[J07] 比较两个日期
来源：http://bpd.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://sic.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ean.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://tea.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://imz.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://flm.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pqf.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://kxh.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://thn.yuanzhike.top

[J08] 提取年月日与星期
来源：http://ise.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://igs.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rmr.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cud.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jzw.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uiv.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rna.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sfk.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nlk.ydjk.org.cn

[J09] 时区处理
来源：http://fih.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kho.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qhh.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dej.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kzx.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xdm.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pxt.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://yyw.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vtd.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://cxr.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://zpb.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fki.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hsn.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pwp.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fim.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tpv.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qwb.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uyz.chenzaomai.com

================================================================================
来源：http://zft.yanxiufei.cn

K. JSON 与序列化
来源：http://wyr.jinqigufen.top

================================================================================
来源：http://apk.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://wyv.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gdx.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://clg.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://pwd.tanke756.top

TS:   JSON.stringify(obj)
来源：http://iog.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fye.yvedp.cn

Go:   json.Marshal(obj)
来源：http://vqz.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ehe.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://aio.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://smx.ydzc1.top

Py:   json.loads(s)
来源：http://zou.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zhm.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://lvd.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://hah.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ghk.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://hck.aizwys.cn

Ruby: JSON.parse(s)
来源：http://dll.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tjk.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://gkv.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://omt.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wed.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://chp.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://owz.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cje.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jed.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://qqx.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bbd.andypj.xyz

[K04] 读取 JSON 文件
来源：http://kxe.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://khu.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jbj.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xhr.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xpn.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lbw.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tek.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nls.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qxo.fehbvm.com

[K05] 深拷贝对象
来源：http://wep.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://sho.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://qzh.sysykeji.top

JS:   structuredClone(obj)
来源：http://ouj.sweek.top

TS:   structuredClone(obj)
来源：http://nqi.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ihm.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://swp.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vdu.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oru.c1oappe.top

[K06] 解析 URL 查询串
来源：http://yik.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://brd.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qem.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oat.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gkn.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dzh.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jom.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ini.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lxo.hongshengwenyu.top

[K07] 进制转换
来源：http://qna.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://agk.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qgl.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://trl.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmr.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cxq.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pof.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kvk.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ztd.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://tir.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://tax.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fte.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://bsf.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://reo.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cvh.cdnleiting.top

Go:   encoding/gob
来源：http://qbk.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://esa.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kua.xylfe.cn

================================================================================
来源：http://plb.fengsongda.top


<!-- 参考信息 -->