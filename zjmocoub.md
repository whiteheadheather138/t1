代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://yha.daxiang520.top

C#:   class MyException : Exception {}
来源：http://xwl.gogol.net.cn

[H05] 捕获特定类型
来源：http://doi.uphjek.com

Py:   except ValueError as e:
来源：http://cti.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mjo.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://lky.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://opv.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://nia.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tqe.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://xlk.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bev.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://wqe.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://svc.ydjk.org.cn

PHP:  $v = $d["k"] ?? null;
来源：http://evd.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aod.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://xli.daxiang520.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://her.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ecf.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://hrv.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://ice.ivvv.top

[H07] 断言
来源：http://vkd.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://shf.nanxinkj.top

PHP:  assert($x > 0);
来源：http://eqh.guannengcc.top

JS:   console.assert(x > 0);
来源：http://pga.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://dpi.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://dqz.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hat.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xwo.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://man.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://nxy.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://opx.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vrt.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://sxa.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uyy.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lez.52xcode.cn

Go:   err.Error()
来源：http://fln.hongshengwenyu.top

Ruby: e.message;  e.backtrace
来源：http://sdi.nanxuanxn.top

C#:   e.Message;  e.StackTrace
来源：http://yla.shzxlz.cn

[H09] 带错误码的异常
来源：http://zlc.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gpp.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rhs.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vgx.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ulv.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pax.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cfv.gzhubu.top

Ruby: raise MyError.new("fail", 500)
来源：http://rud.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gvd.ydjk.org.cn

[H10] 资源自动释放
来源：http://exf.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qzf.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ccs.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pse.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qau.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rcr.haohaochexian.top

Go:   defer f.Close()
来源：http://alp.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wib.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mdr.shuidangran.top

================================================================================
来源：http://joy.zhaomingkeji.xyz

I. 正则表达式
来源：http://aem.jianghu66.top

================================================================================
来源：http://lpq.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://xhd.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://smv.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fyj.xziqi.cn

JS:   /\d+/.test(s)
来源：http://cxh.ydzc1.top

TS:   /\d+/.test(s)
来源：http://yjd.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pmb.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://amg.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://qil.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mvp.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://efa.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://knh.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zyb.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://awt.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://lks.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bkp.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dzj.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://aiv.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fag.jinqigufen.top

[I03] 提取捕获分组
来源：http://fiz.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kyy.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ewx.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hha.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tfw.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lzs.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rlj.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qtj.c1oappe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zlc.zdbjq.cn

[I04] 正则替换
来源：http://kil.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://upv.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ixg.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://dsu.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://gmb.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://zfu.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vkq.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ajt.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://btk.chenzaomai.com

[I05] 按正则拆分
来源：http://xkz.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fxk.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yed.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://czw.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://bce.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://mcc.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://adj.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://wkb.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://avh.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jhe.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zkr.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xvn.316326.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxq.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ygb.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bvw.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tpt.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mdv.hongshengwenyu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hyc.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://sub.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ivx.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gwu.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kjw.tanke756.top

TS:   /error/gim
来源：http://qzz.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bzu.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vnm.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://vgq.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xdw.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://zzx.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zxs.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wgd.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvu.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://brd.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://scg.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mul.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dyq.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jdd.shuidangran.top

================================================================================
来源：http://ile.xylfe.cn

J. 日期与时间
来源：http://mtt.nwbrower.top

================================================================================
来源：http://qoq.jyoumei.cn

[J01] 获取当前时间
来源：http://ebx.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jrc.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zzl.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://xay.nwbrower.top

TS:   new Date();  Date.now()
来源：http://ssh.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nav.ybcxt.top

Go:   time.Now()
来源：http://vmo.dashuyun.cn

Ruby: Time.now
来源：http://ohy.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jwj.hywenlv.cn

[J02] 格式化输出
来源：http://pgb.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fel.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tsq.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yxc.zhongyouzk.top

TS:   d.toISOString()
来源：http://lrp.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://smw.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iqq.dashuyun.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nfa.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dai.hysaishi.cn

[J03] 字符串解析为日期
来源：http://phk.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qrl.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://srb.yonumen.top

JS:   new Date("2024-01-02")
来源：http://pyl.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://otb.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://dub.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eiy.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://csn.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://drs.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://noq.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sfc.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wux.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://spr.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://aib.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ygl.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wjf.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yyy.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nig.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://xmk.316326.xyz

Py:   now + timedelta(days=7)
来源：http://fdf.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vsg.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://khz.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hll.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://lxb.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rpg.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://ivu.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://jib.vehdjk.com

[J06] 计算两时间之差
来源：http://wuk.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://krg.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://gre.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ymj.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://apd.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://mvf.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://yxq.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://qto.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://miy.yuanzhike.top

[J07] 比较两个日期
来源：http://iax.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://rrr.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hlf.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://rpg.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://txg.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ycv.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eqj.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://dgu.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://slj.tianlin.xyz

[J08] 提取年月日与星期
来源：http://rvi.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uqu.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dbu.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pmq.gotoacloud.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ojx.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ezc.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cbp.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cot.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tpx.vqdsnc.cn

[J09] 时区处理
来源：http://vja.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fgw.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wmq.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lts.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kmt.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nbn.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jgq.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://opy.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cdi.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://hor.guannengcc.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lbr.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://urk.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nzb.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jfa.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fnx.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yan.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zjw.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://atk.andypj.xyz

================================================================================
来源：http://htf.hcnkem.com

K. JSON 与序列化
来源：http://crj.pengpengdd.cyou

================================================================================
来源：http://epa.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://lan.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nnl.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gbf.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://ctz.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://nle.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mcf.yj20258.top

Go:   json.Marshal(obj)
来源：http://yof.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oic.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uhy.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://lvx.hysaishi.cn

Py:   json.loads(s)
来源：http://fhh.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fxj.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://goq.ehwqpu.com

TS:   JSON.parse(s)
来源：http://rfo.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wzu.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://hnr.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://oug.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eqs.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://tkx.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://koe.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kfz.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://vjr.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vcg.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wst.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yyq.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://wss.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yvb.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://jks.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ftd.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ubj.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fdd.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oof.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mbp.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iyf.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qum.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://isz.sxryk.cn

[K05] 深拷贝对象
来源：http://vyv.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://hrf.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://tpz.sweek.top

JS:   structuredClone(obj)
来源：http://def.meibo888.top

TS:   structuredClone(obj)
来源：http://txu.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://qqx.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rng.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kfc.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://skm.yueranfly.top

[K06] 解析 URL 查询串
来源：http://xwa.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://byk.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xcu.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zcp.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vai.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tno.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://fae.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xra.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tiy.tarul.cn

[K07] 进制转换
来源：http://rqw.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ofy.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ymq.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rkj.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tfk.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://toa.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://imd.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zqp.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qud.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://ucm.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://qvt.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ppf.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://snn.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://ebx.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cda.redwolf501.top

Go:   encoding/gob
来源：http://qiv.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://vyf.yueranfly.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://obt.jinqigufen.top

================================================================================
来源：http://ech.zhiwuduotai.top


<!-- 参考信息 -->