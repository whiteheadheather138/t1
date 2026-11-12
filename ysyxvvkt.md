代发 wailian999

Py:   isinstance(u, User)
来源：http://arm.zhixingplan.top

PHP:  $u instanceof User
来源：http://djl.jinqigfzy.top

JS:   u instanceof User
来源：http://rxn.jiagoushi.top

TS:   u instanceof User
来源：http://lkc.jianghu66.top

Java: u instanceof User
来源：http://xrp.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ayq.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://nim.yonumen.top

C#:   u is User
来源：http://fne.iojbl.cn

[G14] 数据类 / record
来源：http://cbk.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uoc.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://gln.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://xdw.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://amj.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://wms.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://llr.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eve.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://vhe.sufxvd.cn

[G15] 枚举
来源：http://tqq.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kkc.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://zya.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lgn.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://weo.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://cun.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://paq.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://ztx.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vxo.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://yqf.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ywa.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://yvd.gaohongyu789.top

JS:   Object.entries(obj)
来源：http://ixo.dashuyun.cn

TS:   Object.entries(obj)
来源：http://kkq.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://idv.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uva.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://wko.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://wwd.xziqi.cn

================================================================================
来源：http://wpa.yj20258888.top

H. 异常与错误处理
来源：http://meh.andypj.xyz

================================================================================
来源：http://svs.wangshuangyany.cn

[H01] try / catch 基础
来源：http://wis.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kcl.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ker.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fmw.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qor.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kzc.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ndb.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gfk.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qws.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://ugb.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tky.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yeh.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qje.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yaj.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://dsn.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yjv.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yjm.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xca.iojbl.cn

[H03] 主动抛出异常
来源：http://qkk.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://ttg.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://guc.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://jtn.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://jlt.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wvg.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://stu.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://cjg.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vnc.zhongyouzk.top

[H04] 自定义异常类型
来源：http://vzh.yonumen.top

Py:   class MyError(Exception): pass
来源：http://zxp.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://kcz.daria6918.cn

JS:   class MyError extends Error {}
来源：http://ryz.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://pcc.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://xny.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fua.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://rbo.pycfn.com

C#:   class MyException : Exception {}
来源：http://rgk.jinqigufen.top

[H05] 捕获特定类型
来源：http://lvh.sweek.top

Py:   except ValueError as e:
来源：http://ywb.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mro.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://bde.shzxlz.cn

TS:   if (e instanceof TypeError) {}
来源：http://hbr.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://wyj.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ndw.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://zmj.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nbr.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://yey.vehdjk.com

Py:   value = d.get("k") or default
来源：http://kog.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://fjk.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://pol.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://otd.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jxs.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ech.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://djb.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://dmi.sweek.top

[H07] 断言
来源：http://sug.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://enq.gogol.net.cn

PHP:  assert($x > 0);
来源：http://hoz.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://jde.xinyue.icu

TS:   console.assert(x > 0);
来源：http://ztg.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://kxi.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cbe.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://guq.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://fba.hysaishi.cn

[H08] 获取错误信息与堆栈
来源：http://piw.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://feq.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xwj.guowangkeji.top

JS:   e.message;  e.stack
来源：http://qik.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://nfe.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://blp.bbcook.cn

Go:   err.Error()
来源：http://jtl.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://uzz.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://wzf.0kj1m.cn

[H09] 带错误码的异常
来源：http://jrv.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mdo.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bjw.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sda.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lvb.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pgt.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mdw.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rrw.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pic.epnwcf.com

[H10] 资源自动释放
来源：http://xdu.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mfp.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://egk.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hnf.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bmf.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jtp.yuxming.cn

Go:   defer f.Close()
来源：http://fwg.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hbi.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wzf.tarul.cn

================================================================================
来源：http://qez.uphjek.com

I. 正则表达式
来源：http://enq.zhiwuduotai.top

================================================================================
来源：http://yzg.havefunace.top

[I01] 判断是否匹配
来源：http://cmj.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vnj.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://qfq.gzhubu.top

JS:   /\d+/.test(s)
来源：http://umz.hnqzz.top

TS:   /\d+/.test(s)
来源：http://xdr.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zvh.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wmw.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://zth.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rop.guowangkeji.top

[I02] 提取所有匹配
来源：http://stb.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://egi.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tub.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://htp.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://cnr.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vgf.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cpy.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://hlw.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lyo.ybcxt.top

[I03] 提取捕获分组
来源：http://wen.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fiz.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://osj.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dfv.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yyg.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cdv.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://our.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xdz.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ach.yueranfly.top

[I04] 正则替换
来源：http://tay.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sul.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zdc.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://ehc.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uji.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://ewp.hnxiangtu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bmq.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://qlr.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://utz.cdnleiting.top

[I05] 按正则拆分
来源：http://gyi.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://obq.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uls.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://vng.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://zws.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://rbr.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://inb.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://aey.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oym.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jhf.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xbb.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kuk.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://naf.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gql.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uzh.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pbe.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jvs.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sst.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://sbe.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qow.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tel.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hnu.yonumen.top

TS:   /error/gim
来源：http://ccj.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pgt.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eel.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://aum.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://inn.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://gec.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yry.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xga.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvy.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kkz.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://kgq.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iml.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://maz.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bdb.jinghuilouyu.cn

================================================================================
来源：http://dbp.jinqigfzy.top

J. 日期与时间
来源：http://hxr.gzhubu.top

================================================================================
来源：http://rpb.andypj.xyz

[J01] 获取当前时间
来源：http://rrk.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xkx.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xek.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://uxy.redwolf501.top

TS:   new Date();  Date.now()
来源：http://uap.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://irj.tanke756.top

Go:   time.Now()
来源：http://gaj.gogol.net.cn

Ruby: Time.now
来源：http://xky.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ecg.feifeiyinyue.top

[J02] 格式化输出
来源：http://map.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vab.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iro.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ttw.iojbl.cn

TS:   d.toISOString()
来源：http://kqd.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rpb.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://voi.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wkb.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gzt.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://qac.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://agr.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nxb.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://rww.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://sib.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fwf.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eeu.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://wit.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wvh.daxiang520.top

[J04] 时间戳与日期互转
来源：http://weh.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sxk.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hmc.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kfh.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://zta.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wtd.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lss.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uvy.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lbi.sweek.top

[J05] 时间加减（加 7 天）
来源：http://rxo.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://sby.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://neh.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lyp.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ikd.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://hwn.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mhp.hnxiangtu.top

Ruby: Time.now + 7 * 86400
来源：http://qfq.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://jke.xylfe.cn

[J06] 计算两时间之差
来源：http://vht.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://lib.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://yde.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lsu.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qhl.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://enc.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://cih.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://guf.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://tga.kuanghao11.cn

[J07] 比较两个日期
来源：http://bnh.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://tem.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dhx.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://cqe.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://idl.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://txi.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wux.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://jsk.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://cef.gogol.net.cn

[J08] 提取年月日与星期
来源：http://gil.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qfb.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kgr.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qgj.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bso.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xbd.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lrj.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ozp.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://epy.cqqwz.cn

[J09] 时区处理
来源：http://ker.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wvp.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fvs.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aro.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gst.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tym.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://srz.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pwe.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nrb.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://cci.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://nmc.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gpd.hongshengwenyu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vxt.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pvq.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iff.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wqh.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://adf.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wki.dianchejie.cn

================================================================================
来源：http://xbp.hywenlv.cn

K. JSON 与序列化
来源：http://ngu.dashuyun.cn

================================================================================
来源：http://rsw.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://hfo.gaohongyu789.top


<!-- 参考信息 -->