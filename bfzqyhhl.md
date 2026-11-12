代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://kjp.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://gkj.xinyue.icu

[H05] 捕获特定类型
来源：http://anm.chenlongwang.top

Py:   except ValueError as e:
来源：http://vkf.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://etn.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://sqm.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://xsi.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://sml.hesvh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cvq.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://sao.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dsv.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://vfq.mhx1999.top

Py:   value = d.get("k") or default
来源：http://hsc.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://lmc.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://dol.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://czm.ydjk.org.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qzs.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xlp.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://dtz.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://hxz.xziqi.cn

[H07] 断言
来源：http://cyh.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://mwe.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://bdf.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://sjo.yongpay.top

TS:   console.assert(x > 0);
来源：http://aox.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://wua.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rug.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://kzo.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://euo.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://nzc.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://kxk.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xxe.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://swh.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://lqc.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nca.yvedp.cn

Go:   err.Error()
来源：http://ges.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://qqu.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://jnz.xziqi.cn

[H09] 带错误码的异常
来源：http://jhe.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ktx.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ojk.tian-w.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tyt.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iwg.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wim.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yxs.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://qby.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fnz.mhx1999.top

[H10] 资源自动释放
来源：http://mee.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://caq.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oze.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nhz.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vtz.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hzp.316326.xyz

Go:   defer f.Close()
来源：http://gps.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pow.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ftl.dashuyun.cn

================================================================================
来源：http://llp.hesvh.cn

I. 正则表达式
来源：http://kxj.havefunace.top

================================================================================
来源：http://xbz.gogol.net.cn

[I01] 判断是否匹配
来源：http://ywv.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ivs.sjlbkw.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lsf.yj20258888.top

JS:   /\d+/.test(s)
来源：http://vdw.316326.xyz

TS:   /\d+/.test(s)
来源：http://aco.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://thh.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hyd.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://ijm.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dez.hcnkem.com

[I02] 提取所有匹配
来源：http://uzj.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://api.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nvn.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dgc.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://vpo.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tai.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lee.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://haf.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cym.pycfn.com

[I03] 提取捕获分组
来源：http://hxu.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tgm.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jaz.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ivj.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dyp.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pqn.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uhc.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jlm.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lwb.meibo888.top

[I04] 正则替换
来源：http://ndv.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://poh.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ipu.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://wzh.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://ltw.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://pbr.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mji.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kch.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ike.gotoacloud.top

[I05] 按正则拆分
来源：http://muy.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://omt.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://asz.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://cke.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://wkk.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://ien.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gbd.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://cfj.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dyc.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rpm.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qay.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://frv.316326.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jum.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dio.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ums.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lxn.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nxg.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://clb.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://rds.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lef.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oui.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://huw.yj20258.top

TS:   /error/gim
来源：http://gsw.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://add.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cab.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://svd.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tiu.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://xyl.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qvf.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vsu.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rgp.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kjm.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://bvf.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eqj.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cko.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iuv.daxiang520.top

================================================================================
来源：http://nwa.mhx1999.top

J. 日期与时间
来源：http://ame.mhx1999.top

================================================================================
来源：http://rxf.vqdsnc.cn

[J01] 获取当前时间
来源：http://xer.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mzu.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hdx.uphjek.com

JS:   new Date();  Date.now()
来源：http://dio.birdmap.top

TS:   new Date();  Date.now()
来源：http://jkq.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qpy.aizwys.cn

Go:   time.Now()
来源：http://xup.dashuyun.cn

Ruby: Time.now
来源：http://wuq.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pnw.316326.xyz

[J02] 格式化输出
来源：http://mfr.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://suj.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qck.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vhc.yongpay.top

TS:   d.toISOString()
来源：http://krh.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xdu.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mee.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vhb.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xpf.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://gvb.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rxs.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://whu.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://ebk.316326.xyz

TS:   new Date("2024-01-02")
来源：http://vmx.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mod.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gck.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://myz.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jgl.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://usd.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lfg.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ode.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://djo.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://awr.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qve.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kbw.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jra.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kyx.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://clw.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://krr.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://own.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://roh.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jdh.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://tla.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iyk.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://hxk.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wns.sweek.top

[J06] 计算两时间之差
来源：http://xot.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://ekx.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://wzs.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qfg.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dxh.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://eos.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://iti.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://owp.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://ttr.tian-w.cn

[J07] 比较两个日期
来源：http://rgw.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://ixy.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zvo.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://kof.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pan.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://thy.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fry.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oaz.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://moq.hnqzz.top

[J08] 提取年月日与星期
来源：http://sds.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jof.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vdm.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mcz.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dth.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://par.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eqo.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zsu.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lwu.gotoacloud.top

[J09] 时区处理
来源：http://tqr.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://grf.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ybl.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ziu.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bcn.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rna.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qtt.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://uvs.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zsn.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://och.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ivg.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://clh.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vys.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://run.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://isf.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brx.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cju.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iia.wangdashe.top

================================================================================
来源：http://ofh.yueranfly.top

K. JSON 与序列化
来源：http://sjj.52xcode.cn

================================================================================
来源：http://wqs.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://xty.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lpe.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zuu.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://ilh.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://udr.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://txg.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://wsq.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://xvl.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fzv.fehbvm.com

[K02] JSON 字符串转对象
来源：http://ojd.zdbjq.cn

Py:   json.loads(s)
来源：http://gii.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fvs.yj202588.top

JS:   JSON.parse(s)
来源：http://aac.yj202588.top

TS:   JSON.parse(s)
来源：http://uaw.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rmh.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://nhw.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://ove.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hey.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://xzi.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ouw.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uwu.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fuu.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yvb.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dqm.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cle.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://aou.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://twk.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://gny.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bli.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oxk.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://usz.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dkw.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iph.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aas.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://csf.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cra.c1oappe.top

[K05] 深拷贝对象
来源：http://uld.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://jrz.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://uhk.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://fbt.ctjpmb.com

TS:   structuredClone(obj)
来源：http://utc.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sar.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zto.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://isi.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bix.daria6918.cn

[K06] 解析 URL 查询串
来源：http://jhl.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ezz.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cup.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jqa.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bez.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iri.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oxx.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://idi.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gev.cheryme.top

[K07] 进制转换
来源：http://cki.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uul.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lck.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rje.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ckv.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bgr.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gkm.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qtr.fehbvm.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pjn.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://guf.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://bvr.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yzy.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://lkw.0kj1m.cn

TS:   v8.serialize(obj)        // Node
来源：http://bqz.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dhq.yvedp.cn

Go:   encoding/gob
来源：http://yjn.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://uvt.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ygd.shanyushiyangtech.top

================================================================================
来源：http://gxo.ydzc1.top


<!-- 参考信息 -->