代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oph.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://epu.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zqf.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fhf.ppjwa.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sdh.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pgd.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://klz.redwolf501.top

[H02] finally / ensure 收尾
来源：http://hju.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://slw.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ghg.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ujy.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ocz.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wed.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vkb.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wiy.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xov.yfazqb.com

[H03] 主动抛出异常
来源：http://sii.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://ceh.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xhk.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://tdz.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://dml.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jws.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xbz.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://mca.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://dmz.vehdjk.com

[H04] 自定义异常类型
来源：http://xsr.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://uqw.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://gjh.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://ftx.havefunace.top

TS:   class MyError extends Error {}
来源：http://cus.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://pif.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://djg.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://ckw.daxiang520.top

C#:   class MyException : Exception {}
来源：http://rhh.jianghu66.top

[H05] 捕获特定类型
来源：http://arq.hfpthk.cn

Py:   except ValueError as e:
来源：http://vmm.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ufb.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://wqm.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://uan.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://zyt.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://glm.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://dgr.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://crx.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://bcw.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://rcn.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://iav.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cad.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hvd.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rfm.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bqu.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://nzp.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://dzt.cucudq.cn

[H07] 断言
来源：http://iww.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://odv.andypj.xyz

PHP:  assert($x > 0);
来源：http://hde.cheryme.top

JS:   console.assert(x > 0);
来源：http://ofz.yueranfly.top

TS:   console.assert(x > 0);
来源：http://fdd.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://wpg.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yxi.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bxh.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://kwo.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://frx.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://hyh.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pbf.redwolf501.top

JS:   e.message;  e.stack
来源：http://nlm.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://blj.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wgd.nanxuanxn.top

Go:   err.Error()
来源：http://uvu.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://bmd.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://gpg.pycfn.com

[H09] 带错误码的异常
来源：http://mnx.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vqt.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://nvg.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fxx.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xpd.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qus.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gmc.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://xjq.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kgv.sjlbkw.cn

[H10] 资源自动释放
来源：http://goa.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hrq.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qqh.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cry.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://txh.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mcw.gotoacloud.top

Go:   defer f.Close()
来源：http://tlb.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yon.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jfa.gogol.net.cn

================================================================================
来源：http://ftx.yj20258888.top

I. 正则表达式
来源：http://bcu.jinqigfzy.top

================================================================================
来源：http://cyh.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://wdk.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ayp.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://quw.hesvh.cn

JS:   /\d+/.test(s)
来源：http://yym.cashguo.top

TS:   /\d+/.test(s)
来源：http://xgv.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mtn.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://imp.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://yym.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mwt.yuanzhike.top

[I02] 提取所有匹配
来源：http://whj.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://omz.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mej.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://avv.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://qjs.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hmo.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jqw.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://vdc.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vqp.yueranfly.top

[I03] 提取捕获分组
来源：http://wpb.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bbu.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nnr.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jhx.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ulr.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dqy.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://api.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wca.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ysl.fehbvm.com

[I04] 正则替换
来源：http://gqc.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cyp.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vxv.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://pkm.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mtq.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://qew.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vfq.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gqh.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xbo.cucudq.cn

[I05] 按正则拆分
来源：http://wha.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bwj.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gzw.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://wbb.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://qwl.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://lys.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bqf.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://etf.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bav.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rjv.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rhd.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://chx.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mcy.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kim.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vvs.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dyj.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xyg.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://our.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://klf.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hvb.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://stz.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wfl.0kj1m.cn

TS:   /error/gim
来源：http://ajw.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lyd.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wyb.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://kkp.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lqk.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://fwq.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bjy.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xfy.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fok.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xzj.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ifz.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://trc.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hhs.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://laj.cashguo.top

================================================================================
来源：http://fyk.gotoacloud.top

J. 日期与时间
来源：http://wyu.zhaomingkeji.xyz

================================================================================
来源：http://hjs.tian-w.cn

[J01] 获取当前时间
来源：http://jed.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://raz.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://usg.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://kzc.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://vlu.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ghe.haohaochexian.top

Go:   time.Now()
来源：http://koz.aibaodan.cn

Ruby: Time.now
来源：http://nxy.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aqx.sjlbkw.cn

[J02] 格式化输出
来源：http://jka.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://snc.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lut.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lqq.jyoumei.cn

TS:   d.toISOString()
来源：http://jmn.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wxk.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eko.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jmp.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pck.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://yiz.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tjr.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pjj.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://nve.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://jwf.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://fjx.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://buu.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://bct.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mqu.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://dgl.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kzf.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://arg.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://peo.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tzc.dianchejie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vof.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pby.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qnm.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lwo.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://rkl.jyoumei.cn

Py:   now + timedelta(days=7)
来源：http://wqt.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iui.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hzu.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wfn.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://fwu.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kuw.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://ysw.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://txd.fengsongda.top

[J06] 计算两时间之差
来源：http://ksg.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://qts.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://vow.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tiy.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gmh.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://ohn.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://qbu.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://dzv.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://csz.tian-w.cn

[J07] 比较两个日期
来源：http://inx.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://cnl.meibo888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://txh.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://qfg.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://hut.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hqr.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pak.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://qmp.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://esf.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://gkz.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eyr.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fgb.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://msz.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fvf.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jhv.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yxj.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ucj.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wll.shangyingyoupin.top

[J09] 时区处理
来源：http://knx.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pmj.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://how.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jxu.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sab.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dbu.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uym.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ygl.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ysf.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://ejn.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://fgx.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cjs.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://see.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pvr.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wom.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wkv.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gjd.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ijs.zhaomingkeji.xyz

================================================================================
来源：http://big.wangdashe.top

K. JSON 与序列化
来源：http://zun.ydzc1.top

================================================================================
来源：http://dqj.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://dkd.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nwp.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://teh.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://fxf.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://cdr.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qal.yvedp.cn

Go:   json.Marshal(obj)
来源：http://zwg.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://cky.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rif.yongpay.top

[K02] JSON 字符串转对象
来源：http://nuu.svipenyu.cn

Py:   json.loads(s)
来源：http://kqd.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pxo.yfazqb.com

JS:   JSON.parse(s)
来源：http://hrk.zycfv.cn

TS:   JSON.parse(s)
来源：http://yuw.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mtt.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://ahr.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://lxk.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ddu.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://yuu.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fxj.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jxi.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yya.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wde.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dzy.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://olm.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://ufw.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lzx.tanke756.top

[K04] 读取 JSON 文件
来源：http://ggx.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ihs.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zju.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cka.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yqs.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mhg.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://crl.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://zrp.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tqz.yongpay.top

[K05] 深拷贝对象
来源：http://als.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://lfu.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://apq.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://bmx.epnwcf.com

TS:   structuredClone(obj)
来源：http://fex.0kj1m.cn


<!-- 参考信息 -->