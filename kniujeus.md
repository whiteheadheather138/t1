代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://mvs.bjfxy.top

Java: record User(String name, int age) {}
来源：http://rag.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://oin.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rhc.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://rbl.zhijiandao.cn

[G15] 枚举
来源：http://vma.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://exm.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zec.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yfj.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vcj.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://ima.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pco.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://kgx.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://opy.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://dyu.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xsj.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://llj.52xcode.cn

JS:   Object.entries(obj)
来源：http://uof.cashguo.top

TS:   Object.entries(obj)
来源：http://qze.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kyu.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gvg.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://unn.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://cfh.snrcjt.cn

================================================================================
来源：http://spl.tianlin.xyz

H. 异常与错误处理
来源：http://tib.chenzaomai.com

================================================================================
来源：http://dsz.yfazqb.com

[H01] try / catch 基础
来源：http://jyw.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vit.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jwo.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bzd.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://csf.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ipt.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rif.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hzm.hfpthk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mlz.havefunace.top

[H02] finally / ensure 收尾
来源：http://qsm.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://dvm.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yyy.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ktv.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pds.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://rrv.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://beu.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qls.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://fij.cdnleiting.top

[H03] 主动抛出异常
来源：http://ell.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://nwj.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ffu.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://zls.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://hkj.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://afd.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sor.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://iet.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://xnr.sxryk.cn

[H04] 自定义异常类型
来源：http://nym.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://nno.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rqm.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://bhw.fehbvm.com

TS:   class MyError extends Error {}
来源：http://yed.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://lnn.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pwa.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://qoi.hnqzz.top

C#:   class MyException : Exception {}
来源：http://frq.c1oappe.top

[H05] 捕获特定类型
来源：http://exd.wangdashe.top

Py:   except ValueError as e:
来源：http://kuf.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://akq.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://loa.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://wgm.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://dim.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xwv.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://zzp.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jyy.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://pdv.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://pjh.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yzk.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://eel.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://qim.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://odm.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://clt.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://kyd.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://puj.sxryk.cn

[H07] 断言
来源：http://oux.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://ubh.mhx1999.top

PHP:  assert($x > 0);
来源：http://jgi.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://aqj.xuanzx.com

TS:   console.assert(x > 0);
来源：http://meh.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://tki.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fsu.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://urq.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://sfi.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://day.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://frz.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://klo.yanxiufei.cn

JS:   e.message;  e.stack
来源：http://fzq.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hyn.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://drg.gzhubu.top

Go:   err.Error()
来源：http://adx.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://gkd.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://icq.cheryme.top

[H09] 带错误码的异常
来源：http://rjt.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://awc.fzhhl.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zqo.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xon.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ezu.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ctb.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://axr.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rpd.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bbc.jlsjyb.cn

[H10] 资源自动释放
来源：http://vlx.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mlf.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wng.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bsg.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://svu.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ldz.hywenlv.cn

Go:   defer f.Close()
来源：http://ykj.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tmc.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vtd.zycfv.cn

================================================================================
来源：http://ref.quarkkingdee.top

I. 正则表达式
来源：http://iln.hongshengwenyu.top

================================================================================
来源：http://cgw.zhengqikj.top

[I01] 判断是否匹配
来源：http://ciz.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rxr.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eag.birdmap.top

JS:   /\d+/.test(s)
来源：http://swl.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://esa.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xmi.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qrv.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://xsn.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://awo.xylfe.cn

[I02] 提取所有匹配
来源：http://ktt.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://prr.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fbi.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zbc.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://syr.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://luv.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jgx.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://ynh.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nud.daria6918.cn

[I03] 提取捕获分组
来源：http://xma.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mva.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bud.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hnj.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vnm.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ytf.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iol.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://doz.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pbx.yanxiufei.cn

[I04] 正则替换
来源：http://vgz.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gjj.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nai.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://voe.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://nzk.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://ziw.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ejn.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yfl.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tkk.xziqi.cn

[I05] 按正则拆分
来源：http://uiw.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tjd.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://orn.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://tyq.yj20258.top

TS:   s.split(/\s*,\s*/)
来源：http://bzh.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://umy.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ohb.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://bpj.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://boq.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ffb.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xtf.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uve.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ehe.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oco.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sjk.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://njj.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tqf.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bnu.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://xcg.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://avs.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qby.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bxo.aibaodan.cn

TS:   /error/gim
来源：http://swf.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vib.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yto.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://ipk.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ggi.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://ztt.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zig.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aan.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtn.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dhj.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qfb.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://evh.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://whx.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ghy.zhijiandao.cn

================================================================================
来源：http://sbi.shzxlz.cn

J. 日期与时间
来源：http://jre.zhixingplan.top

================================================================================
来源：http://hmk.yongpay.top

[J01] 获取当前时间
来源：http://eve.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wqw.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://obn.daria6918.cn

JS:   new Date();  Date.now()
来源：http://kcn.316326.xyz

TS:   new Date();  Date.now()
来源：http://mfr.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pbs.yongpay.top

Go:   time.Now()
来源：http://oyo.meibo888.top

Ruby: Time.now
来源：http://fee.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kmv.dianchejie.cn

[J02] 格式化输出
来源：http://nhm.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kaf.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hqm.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wwz.haohaochexian.top

TS:   d.toISOString()
来源：http://ofc.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://scj.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dge.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qnr.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uvy.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://zkp.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xpv.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aoi.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://mow.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://fwp.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://hyg.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sef.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://bms.haohaochexian.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uzm.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://nvf.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://glz.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gjd.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blq.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gmf.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yew.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ogv.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gyr.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jii.hesvh.cn

[J05] 时间加减（加 7 天）
来源：http://xmq.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://kgg.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://tum.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lfw.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cbp.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://eyg.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vev.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://dmy.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://amt.daxiang520.top

[J06] 计算两时间之差
来源：http://cdf.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://shj.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://exe.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hyr.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qqp.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://knt.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://cks.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://wjx.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://ndr.yuxming.cn

[J07] 比较两个日期
来源：http://ukb.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://zzn.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vxh.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://bsd.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://qzs.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hbo.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pfj.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://ygq.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://omo.jiagoushi.top

[J08] 提取年月日与星期
来源：http://ihm.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hnw.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gcn.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nya.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jud.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hcv.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yhv.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ail.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://meh.ywan-chungtsiang.top

[J09] 时区处理
来源：http://vwb.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rrc.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qwg.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hfn.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxx.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aop.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kud.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://irj.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://viu.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://fsh.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vdk.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://myb.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ghz.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sfx.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://umw.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gie.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lqj.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zrn.haohaochexian.top

================================================================================
来源：http://ltg.shzxlz.cn

K. JSON 与序列化
来源：http://iic.shangyingyoupin.top

================================================================================
来源：http://vjk.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://lku.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://der.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://arn.uphjek.com

JS:   JSON.stringify(obj)
来源：http://kpu.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://cep.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pyr.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://oux.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://mqr.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sia.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://evk.0kj1m.cn

Py:   json.loads(s)
来源：http://nos.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xfl.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://egr.ehwqpu.com


<!-- 参考信息 -->