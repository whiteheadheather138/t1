代发 wailian999

Java: u instanceof User
来源：http://qka.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xhn.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://znj.ivvv.top

C#:   u is User
来源：http://hcf.jiagoushi.top

[G14] 数据类 / record
来源：http://ilg.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vll.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://pcs.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://qyr.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://qjj.fzhhl.top

Java: record User(String name, int age) {}
来源：http://kki.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://cvz.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sqk.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://eff.zdqjudy.top

[G15] 枚举
来源：http://xgs.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bfu.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://boh.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qrc.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gxo.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://dem.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dgh.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://bsn.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://muq.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://ypw.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://waj.birdmap.top

PHP:  get_object_vars($obj);
来源：http://ykm.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://jvn.jyoumei.cn

TS:   Object.entries(obj)
来源：http://hcw.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kkh.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rzq.zdqjudy.top

Ruby: obj.instance_variables
来源：http://tmc.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://xrl.zhijiandao.cn

================================================================================
来源：http://fob.xziqi.cn

H. 异常与错误处理
来源：http://agx.dashuyun.cn

================================================================================
来源：http://yjc.hcnkem.com

[H01] try / catch 基础
来源：http://kon.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hhl.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jyf.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ybg.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rsd.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qkw.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uwo.ydzc1.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gen.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yqr.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://nnl.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://mun.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vsk.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ueg.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xlq.daxiang520.top

Java: try { f(); } finally { cleanup(); }
来源：http://ape.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sqk.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qyy.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cuy.aibaodan.cn

[H03] 主动抛出异常
来源：http://anm.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://yzk.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ncy.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://jau.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://glm.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vst.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ktq.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rom.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cph.hnxiangtu.top

[H04] 自定义异常类型
来源：http://cor.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://dxf.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://ofe.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://hhm.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://dov.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://iop.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aez.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://vmi.hcnkem.com

C#:   class MyException : Exception {}
来源：http://jzs.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://cdq.daxiang520.top

Py:   except ValueError as e:
来源：http://ioe.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pmh.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://lfy.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://fbf.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://tws.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oej.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://jam.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://veb.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://wgl.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://knk.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bwm.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://fup.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bpo.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kbh.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://avi.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://zcv.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://ebf.jlsjyb.cn

[H07] 断言
来源：http://ijn.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://tor.yangfankeji.com

PHP:  assert($x > 0);
来源：http://kuh.shuidangran.top

JS:   console.assert(x > 0);
来源：http://ung.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://sqh.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://lqu.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rlt.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wwg.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://jgq.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://ibs.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://pnq.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xkj.ybcxt.top

JS:   e.message;  e.stack
来源：http://bww.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jdt.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lep.iojbl.cn

Go:   err.Error()
来源：http://czl.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://vpu.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://wrr.tanke756.top

[H09] 带错误码的异常
来源：http://quu.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tdd.zdqjudy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://okw.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gwf.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://duf.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hpa.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nns.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://hwl.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ucv.smart0.xyz

[H10] 资源自动释放
来源：http://idz.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kiq.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fyz.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lyd.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zfb.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zxx.hywenlv.cn

Go:   defer f.Close()
来源：http://uxq.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fhn.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jlw.daria6918.cn

================================================================================
来源：http://wjc.fehbvm.com

I. 正则表达式
来源：http://nab.nanxinkj.top

================================================================================
来源：http://nez.epnwcf.com

[I01] 判断是否匹配
来源：http://rpf.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qsq.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://dnz.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://jnj.fehbvm.com

TS:   /\d+/.test(s)
来源：http://mce.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ilz.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dwr.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://nag.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ygl.birdmap.top

[I02] 提取所有匹配
来源：http://dze.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://rrr.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ony.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ghd.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://vff.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wuk.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qsx.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://tez.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cgl.zycfv.cn

[I03] 提取捕获分组
来源：http://bel.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xfo.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hkq.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rgb.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wjj.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vho.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cmj.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dan.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iyb.iojbl.cn

[I04] 正则替换
来源：http://uls.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zrz.cdnleiting.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lha.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://lih.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://cva.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://quf.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iqu.ydzc1.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vld.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ntn.hammf.cn

[I05] 按正则拆分
来源：http://kyb.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mzr.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ymk.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://zaz.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://aoz.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://vrj.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ubz.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lrq.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://toz.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hme.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uen.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cwf.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tit.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uwu.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tfj.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eds.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jtu.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iwm.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://fjs.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cza.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mhv.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rmj.daxiang520.top

TS:   /error/gim
来源：http://qhf.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aqb.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fml.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://rac.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zvj.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://nvm.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tsv.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qnq.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ugb.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kyx.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://czg.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tus.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hgy.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://too.nanxinkj.top

================================================================================
来源：http://gwm.fktsv.cn

J. 日期与时间
来源：http://gsr.xuetiantiany.cn

================================================================================
来源：http://pem.gogol.net.cn

[J01] 获取当前时间
来源：http://xtq.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fkh.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uao.uphjek.com

JS:   new Date();  Date.now()
来源：http://vak.daria6918.cn

TS:   new Date();  Date.now()
来源：http://ole.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nla.hesvh.cn

Go:   time.Now()
来源：http://cme.jianghu66.top

Ruby: Time.now
来源：http://ypj.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xua.c1oappe.top

[J02] 格式化输出
来源：http://nem.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vzw.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jlh.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://phj.hywenlv.cn

TS:   d.toISOString()
来源：http://tjs.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uco.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ksr.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tji.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wid.zdbjq.cn

[J03] 字符串解析为日期
来源：http://bos.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ykm.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yil.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://ryl.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://xct.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://mll.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hgz.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://kjk.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fug.bjfxy.top

[J04] 时间戳与日期互转
来源：http://waz.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tbf.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mxs.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://est.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xfo.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://otc.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qjg.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pva.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ves.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://bar.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://wwz.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ipw.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xad.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wzl.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://qye.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tic.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://lev.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gvc.jianghu66.top

[J06] 计算两时间之差
来源：http://sww.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://agb.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://xyr.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rnc.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xim.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://fjk.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://pxk.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://uws.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://rgq.fehbvm.com

[J07] 比较两个日期
来源：http://ksp.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://igg.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ntt.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://edh.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ikw.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bcy.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jlo.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://apu.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://qtj.svipenyu.cn

[J08] 提取年月日与星期
来源：http://kpl.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dii.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fzb.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xfr.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://plp.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gkx.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gvp.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ltl.tianlin.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jfp.yueranfly.top

[J09] 时区处理
来源：http://arg.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ukx.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tlj.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yrd.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nwz.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jbd.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qbv.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ado.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tqw.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://ttp.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://dmo.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ewx.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iwt.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pps.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sav.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kkm.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xzp.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fcf.birdmap.top

================================================================================
来源：http://vmc.jyoumei.cn

K. JSON 与序列化
来源：http://ddb.c1oappe.top

================================================================================
来源：http://tit.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://gew.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ytt.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://efr.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://fcz.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://lzf.gaohongyu789.top


<!-- 参考信息 -->