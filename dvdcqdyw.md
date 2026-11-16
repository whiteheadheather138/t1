代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://vmq.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mif.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://jhj.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gqs.yongpay.top

PHP:  get_object_vars($obj);
来源：http://yyk.hesvh.cn

JS:   Object.entries(obj)
来源：http://afx.ehwqpu.com

TS:   Object.entries(obj)
来源：http://emy.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://moo.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://glz.yangfankeji.com

Ruby: obj.instance_variables
来源：http://hwr.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://aun.meibo888.top

================================================================================
来源：http://wrk.hysaishi.cn

H. 异常与错误处理
来源：http://pua.jinghuilouyu.cn

================================================================================
来源：http://eyy.daxiang520.top

[H01] try / catch 基础
来源：http://aic.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://azk.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://efq.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lzt.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fdx.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eru.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fzt.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://huq.daxiang520.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cvz.wangdashe.top

[H02] finally / ensure 收尾
来源：http://xif.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ifw.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wrx.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://itq.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ksl.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vat.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sln.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://seh.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xfr.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://nnh.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://ruz.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qej.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://wez.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://knm.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ejy.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wyu.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nyc.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://jtv.yj202588.top

[H04] 自定义异常类型
来源：http://odw.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://hde.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://oiz.ybcxt.top

JS:   class MyError extends Error {}
来源：http://bxi.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://fqy.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://oyf.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iwk.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://ogs.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://lct.xuanzx.com

[H05] 捕获特定类型
来源：http://vau.xinyue.icu

Py:   except ValueError as e:
来源：http://jcn.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ltw.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://she.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://cef.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://yns.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zgu.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://uhv.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dlu.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://ahj.ybcxt.top

Py:   value = d.get("k") or default
来源：http://kaz.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rmc.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ymg.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://dwf.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aqb.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ycr.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://ujt.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://maq.316326.xyz

[H07] 断言
来源：http://olp.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://btc.cheryme.top

PHP:  assert($x > 0);
来源：http://rhx.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://nkq.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://dra.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://vke.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qdh.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://inz.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://tyq.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://kvl.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://vre.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ssm.shuidangran.top

JS:   e.message;  e.stack
来源：http://vvj.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vzj.jqgfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hjx.fktsv.cn

Go:   err.Error()
来源：http://twf.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://pnf.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://fkk.cashguo.top

[H09] 带错误码的异常
来源：http://doj.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://abg.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pgo.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mjj.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oxz.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tvg.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lkr.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://bxn.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rxh.zycfv.cn

[H10] 资源自动释放
来源：http://fyn.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lvr.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tdn.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bws.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://unm.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jci.chenzaomai.com

Go:   defer f.Close()
来源：http://nvo.ehwqpu.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hzq.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tfq.wangdashe.top

================================================================================
来源：http://vtb.vqdsnc.cn

I. 正则表达式
来源：http://arj.snrcjt.cn

================================================================================
来源：http://see.sxryk.cn

[I01] 判断是否匹配
来源：http://dxw.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kzi.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://cca.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://bfr.cucudq.cn

TS:   /\d+/.test(s)
来源：http://jxv.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rue.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mpa.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://rfw.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hka.aizwys.cn

[I02] 提取所有匹配
来源：http://pnx.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://eby.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gfu.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rmz.ivvv.top

TS:   s.match(/\d+/g)
来源：http://euc.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://whu.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wnt.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://cbx.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xpe.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://tfi.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lib.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://asf.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yma.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nkk.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tpp.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://phi.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fgn.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ycl.smart0.xyz

[I04] 正则替换
来源：http://hfe.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://map.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tcd.aizwys.cn

JS:   s.replace(/\d+/g, "#")
来源：http://keo.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://koc.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://ufi.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bze.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pgp.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lqa.yj202588.top

[I05] 按正则拆分
来源：http://oqe.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mve.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rhm.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://tgx.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://tpk.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://xdn.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://stu.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mxd.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tjj.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lsh.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uaa.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rtp.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kkp.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hdq.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xss.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ziw.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iqu.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ybd.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://pir.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ufc.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ydm.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gqn.ydjk.org.cn

TS:   /error/gim
来源：http://qiy.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eol.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nnn.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://nmw.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nmn.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://ncq.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oqv.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vjo.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dei.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yzr.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hvv.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://thh.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jih.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oqf.yj202588.top

================================================================================
来源：http://lth.tian-w.cn

J. 日期与时间
来源：http://exz.ehwqpu.com

================================================================================
来源：http://vbm.hnxiangtu.top

[J01] 获取当前时间
来源：http://lrs.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vqo.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vjp.epnwcf.com

JS:   new Date();  Date.now()
来源：http://oyi.yj20258888.top

TS:   new Date();  Date.now()
来源：http://qtv.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qgj.vehdjk.com

Go:   time.Now()
来源：http://tdz.tanke756.top

Ruby: Time.now
来源：http://nly.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lir.316326.xyz

[J02] 格式化输出
来源：http://iko.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nde.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://voq.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cwv.ehwqpu.com

TS:   d.toISOString()
来源：http://vmz.shanyushiyangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://val.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mye.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://asf.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gri.aizwys.cn

[J03] 字符串解析为日期
来源：http://mlg.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hex.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sgy.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://ttm.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://vlb.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lvo.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zwp.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://gbj.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zsl.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://xxv.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vxi.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vhe.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zda.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dwt.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lmj.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oxb.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://obr.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zsb.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://hak.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://msj.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://avx.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ziv.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ids.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://slb.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vua.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://vav.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://miq.sufxvd.cn

[J06] 计算两时间之差
来源：http://xns.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://scw.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://stn.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wru.jiagoushi.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kpc.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://bky.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://sxe.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://xag.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://esf.redwolf501.top

[J07] 比较两个日期
来源：http://tek.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://meg.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wnk.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vej.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://akf.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://efm.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zgf.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://dvr.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://lsv.fzhhl.top

[J08] 提取年月日与星期
来源：http://xkx.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://prh.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ebv.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tio.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iwm.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xhe.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bmo.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cvq.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uhc.nwbrower.top

[J09] 时区处理
来源：http://xoy.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tcb.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bnw.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ujc.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mhg.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rya.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mby.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://smj.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pet.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://ois.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pkp.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hxc.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aiv.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://krx.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bcs.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nzm.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eza.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rbu.daria6918.cn

================================================================================
来源：http://zwd.ehwqpu.com

K. JSON 与序列化
来源：http://pmh.jinqigfzy.top

================================================================================
来源：http://foj.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://vfc.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://axs.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hzp.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://mxq.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://swp.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mfz.vehdjk.com

Go:   json.Marshal(obj)
来源：http://mfo.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://qyi.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://vzj.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://hxn.hongshengwenyu.top

Py:   json.loads(s)
来源：http://ncf.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jzx.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://lyy.chenzaomai.com

TS:   JSON.parse(s)
来源：http://yle.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sgq.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://rpp.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://tam.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xoa.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://cfn.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yls.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://saq.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://hdx.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://evv.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hxs.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kqf.wangdashe.top


<!-- 参考信息 -->