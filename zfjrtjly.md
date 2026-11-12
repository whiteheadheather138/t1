代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://cju.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://mjc.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://lay.hongshengwenyu.top

[G13] 判断对象类型
来源：http://wxp.hnqzz.top

Py:   isinstance(u, User)
来源：http://ajz.yueranfly.top

PHP:  $u instanceof User
来源：http://dhw.sysykeji.top

JS:   u instanceof User
来源：http://zyw.pycfn.com

TS:   u instanceof User
来源：http://few.tianlin.xyz

Java: u instanceof User
来源：http://ufq.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://dpq.52xcode.cn

Ruby: u.is_a?(User)
来源：http://qwt.nanxuanxn.top

C#:   u is User
来源：http://smr.haohaochexian.top

[G14] 数据类 / record
来源：http://fmh.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lvy.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://tsk.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ntc.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://gub.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://prf.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://abs.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jnx.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://egh.jinghuilouyu.cn

[G15] 枚举
来源：http://ahd.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kym.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://uya.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jjo.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zwa.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://tlj.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://axc.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://sbi.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tkq.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://wmo.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ivb.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://hak.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://erb.birdmap.top

TS:   Object.entries(obj)
来源：http://qer.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yfh.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zxk.snrcjt.cn

Ruby: obj.instance_variables
来源：http://wxm.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://tcx.cucudq.cn

================================================================================
来源：http://dks.aizwys.cn

H. 异常与错误处理
来源：http://jgu.xinyue.icu

================================================================================
来源：http://iyd.xziqi.cn

[H01] try / catch 基础
来源：http://zgq.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dmc.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aic.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xjt.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cye.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ama.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://asv.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dsc.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xzy.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://ety.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://vbr.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kvn.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://epk.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://rbr.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://cyt.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wwm.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ikr.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vhn.gotoacloud.top

[H03] 主动抛出异常
来源：http://xko.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://ale.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ylx.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://ugw.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://yhk.hnqzz.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ica.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pfx.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ogz.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://orm.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://kpd.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://xur.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://cud.nwbrower.top

JS:   class MyError extends Error {}
来源：http://ryc.nanxinkj.top

TS:   class MyError extends Error {}
来源：http://gre.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://fyj.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fcq.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://ylj.birdmap.top

C#:   class MyException : Exception {}
来源：http://opb.daxiang520.top

[H05] 捕获特定类型
来源：http://zos.nanxuanxn.top

Py:   except ValueError as e:
来源：http://xlp.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tqb.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://hgy.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://kdy.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://jto.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tfw.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://kdq.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cdr.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://ett.birdmap.top

Py:   value = d.get("k") or default
来源：http://srr.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://mlv.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mqo.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hiw.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ibi.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fgf.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://nmq.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://rey.zycfv.cn

[H07] 断言
来源：http://mrq.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://gml.birdmap.top

PHP:  assert($x > 0);
来源：http://saj.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://qfm.yj20258888.top

TS:   console.assert(x > 0);
来源：http://lvk.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://eyr.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jlu.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://gxo.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://qie.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://vyi.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://mih.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fpq.tanke756.top

JS:   e.message;  e.stack
来源：http://esm.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hzm.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://ysy.jyoumei.cn

Go:   err.Error()
来源：http://sof.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://pym.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://dpr.chenlongwang.top

[H09] 带错误码的异常
来源：http://fuo.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jdh.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gsl.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://whi.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ald.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iyb.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zcd.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://mrr.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rle.shangyingyoupin.top

[H10] 资源自动释放
来源：http://jmz.ivvv.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://alu.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hcb.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gvc.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ese.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gci.ydjk.org.cn

Go:   defer f.Close()
来源：http://qko.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fvo.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ihl.tarul.cn

================================================================================
来源：http://hih.cucudq.cn

I. 正则表达式
来源：http://ktk.daria6918.cn

================================================================================
来源：http://sgk.yj20258888.top

[I01] 判断是否匹配
来源：http://not.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ffl.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://tcv.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://twj.aizwys.cn

TS:   /\d+/.test(s)
来源：http://uni.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zwa.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yks.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://ggv.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bnr.snrcjt.cn

[I02] 提取所有匹配
来源：http://nmg.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://aek.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cmm.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wmb.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://kkf.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uhw.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ppp.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://ugz.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://prg.jyoumei.cn

[I03] 提取捕获分组
来源：http://eyx.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://auh.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://drj.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qil.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dym.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cdv.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dpw.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gbq.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zau.jinghuilouyu.cn

[I04] 正则替换
来源：http://iak.shuidangran.top

Py:   re.sub(r"\d+", "#", s)
来源：http://snk.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oin.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://wbi.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://nxq.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://voe.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ryl.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dlf.xuanzx.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eaw.tarul.cn

[I05] 按正则拆分
来源：http://rap.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kld.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aio.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://pgv.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://ast.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://chs.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eeq.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://wxq.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vbu.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yll.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gap.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ypa.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bgu.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wrj.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sie.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yjy.gotoacloud.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tww.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zol.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://mwn.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://djx.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jxz.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://apf.nanxinkj.top

TS:   /error/gim
来源：http://iaz.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ops.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://szc.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://urc.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jba.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://cpj.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://whb.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uek.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uwz.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iep.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ssr.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nbb.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ddx.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lxx.hammf.cn

================================================================================
来源：http://byq.haohaochexian.top

J. 日期与时间
来源：http://yel.daria6918.cn

================================================================================
来源：http://ejf.jyoumei.cn

[J01] 获取当前时间
来源：http://aoo.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://osb.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zbh.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://ank.mhx1999.top

TS:   new Date();  Date.now()
来源：http://ejg.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://moq.yj20258888.top

Go:   time.Now()
来源：http://pab.shuidangran.top

Ruby: Time.now
来源：http://etx.pycfn.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lgd.gaohongyu789.top

[J02] 格式化输出
来源：http://wkd.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zam.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hnh.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lvz.wangshuangyany.cn

TS:   d.toISOString()
来源：http://ogo.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vgj.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://idy.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mdq.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fwi.ydzc1.top

[J03] 字符串解析为日期
来源：http://xfb.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gcz.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qcz.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://kqo.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://qzr.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fbx.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iub.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://uev.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://anq.shuidangran.top

[J04] 时间戳与日期互转
来源：http://mxw.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bly.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mta.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fzk.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://wvf.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zcb.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ulu.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tgx.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ayy.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://zqe.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://eed.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://srv.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qez.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://biw.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://ysy.cashguo.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zro.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://gcx.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://qhv.xinyue.icu

[J06] 计算两时间之差
来源：http://usp.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://spl.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://jtf.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jhc.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://glm.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ivk.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://aqv.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://gua.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://dqe.vqdsnc.cn

[J07] 比较两个日期
来源：http://lkt.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://ugj.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ujs.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mxg.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://mrz.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tgp.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yqj.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://mzr.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://wxr.wangdashe.top

[J08] 提取年月日与星期
来源：http://qqz.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tby.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sej.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dlx.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lnk.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cyb.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://czj.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://whs.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ufs.fktsv.cn

[J09] 时区处理
来源：http://rbk.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hwg.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bnz.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxc.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yfp.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gsh.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lcj.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://oiv.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zqx.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://mvh.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://eok.sysykeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zwd.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bwq.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ere.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dcb.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://odh.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ikp.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://chi.daxiang520.top


<!-- 参考信息 -->