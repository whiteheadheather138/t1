代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://vpb.nwbrower.top

JS:   toString() { return this.name; }
来源：http://ipq.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://feg.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://iwo.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hcf.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://qya.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://bef.zhoulong.xyz

[G13] 判断对象类型
来源：http://fvh.sxryk.cn

Py:   isinstance(u, User)
来源：http://kdq.daria6918.cn

PHP:  $u instanceof User
来源：http://qwi.zhixingplan.top

JS:   u instanceof User
来源：http://sxh.jlsjyb.cn

TS:   u instanceof User
来源：http://hfw.bbcook.cn

Java: u instanceof User
来源：http://ffd.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eaf.fzhhl.top

Ruby: u.is_a?(User)
来源：http://apr.jlsjyb.cn

C#:   u is User
来源：http://ito.zycfv.cn

[G14] 数据类 / record
来源：http://dgu.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oab.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://pex.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://ekt.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://hqz.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://zly.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://nxd.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kzx.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://pqv.jqgfzy.top

[G15] 枚举
来源：http://ioj.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hzs.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://tnj.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xgk.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dqe.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://fvs.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ayd.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://hcv.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ffj.hcnkem.com

[G16] 对象转数组 / 字典
来源：http://sla.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xib.hammf.cn

PHP:  get_object_vars($obj);
来源：http://iiy.zycfv.cn

JS:   Object.entries(obj)
来源：http://agw.xziqi.cn

TS:   Object.entries(obj)
来源：http://sud.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yek.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mlo.fengsongda.top

Ruby: obj.instance_variables
来源：http://frm.shanyushiyangtech.top

C#:   // 用反射或 System.Text.Json
来源：http://uil.hnxiangtu.top

================================================================================
来源：http://bog.zhoulong.xyz

H. 异常与错误处理
来源：http://oxx.zhaomingkeji.xyz

================================================================================
来源：http://fqa.feifeiyinyue.top

[H01] try / catch 基础
来源：http://gqm.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://isj.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bzu.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dss.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xza.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yvg.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ehk.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dlu.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lax.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://owd.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zka.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ipg.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ocl.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://coo.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ivx.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://hzr.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gnj.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sqo.cucudq.cn

[H03] 主动抛出异常
来源：http://nsy.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://igr.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://udz.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://jis.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://itj.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dll.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://brj.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jpv.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://juz.shzxlz.cn

[H04] 自定义异常类型
来源：http://kyx.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://dhc.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://rka.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://tgd.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://hwz.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://zpk.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zoa.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://muy.fzhhl.top

C#:   class MyException : Exception {}
来源：http://olw.zhoulong.xyz

[H05] 捕获特定类型
来源：http://rzz.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://vtq.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ehi.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://dki.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://xzh.wangshuangyany.cn

Java: catch (IOException | SQLException e) {}
来源：http://aac.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tuv.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://keu.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lww.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://djz.sxryk.cn

Py:   value = d.get("k") or default
来源：http://xgc.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://joo.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://uce.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hwz.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wdh.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://llb.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://sog.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://wum.bjfxy.top

[H07] 断言
来源：http://tzm.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://lla.fehbvm.com

PHP:  assert($x > 0);
来源：http://owm.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://wzh.yj20258.top

TS:   console.assert(x > 0);
来源：http://dkh.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://dvy.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nby.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://vpb.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://jnl.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://bpt.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://bzj.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gvh.ydzc1.top

JS:   e.message;  e.stack
来源：http://dnp.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://eor.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://fsq.c1oappe.top

Go:   err.Error()
来源：http://jlz.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://ofy.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://vyt.yj202588.top

[H09] 带错误码的异常
来源：http://ycw.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ruu.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rno.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gry.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kjr.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tla.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hol.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://nwy.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cvh.sweek.top

[H10] 资源自动释放
来源：http://myf.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uld.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lpv.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yvx.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vzv.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://twc.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://dph.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uyz.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uyk.jinqigufen.top

================================================================================
来源：http://riy.zhoulong.xyz

I. 正则表达式
来源：http://phj.zhongyouzk.top

================================================================================
来源：http://cjo.jlsjyb.cn

[I01] 判断是否匹配
来源：http://vlb.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uus.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://efi.tanke756.top

JS:   /\d+/.test(s)
来源：http://qgb.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://rga.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vlw.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://abh.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://rgb.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kgz.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://iio.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://izq.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://apk.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cdm.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://dlr.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qcw.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gju.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://fkx.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wpc.ydjk.org.cn

[I03] 提取捕获分组
来源：http://pbz.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nuh.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gju.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://exk.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jak.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yhb.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vdq.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ghm.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://isv.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://oeg.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://qug.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rci.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://hjx.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bkk.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://qcf.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qch.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mga.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xpp.cucudq.cn

[I05] 按正则拆分
来源：http://heo.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oxk.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fpb.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://vqc.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://gfn.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://cgt.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zgp.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://xbo.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://chu.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ryx.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pwh.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yyo.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rev.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://til.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hcd.xylfe.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://woz.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fgq.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://end.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://nkx.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vmb.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vlw.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rih.yvedp.cn

TS:   /error/gim
来源：http://ohr.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yhx.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zmy.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://dbo.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://clz.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://uyl.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pqb.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://out.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dej.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://doo.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vfb.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tzm.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wek.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gpe.sxryk.cn

================================================================================
来源：http://gug.xuetiantiany.cn

J. 日期与时间
来源：http://ibw.feifeiyinyue.top

================================================================================
来源：http://xbj.sufxvd.cn

[J01] 获取当前时间
来源：http://bod.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kwr.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gge.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://yhl.wangdashe.top

TS:   new Date();  Date.now()
来源：http://cfe.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://trx.cdnleiting.top

Go:   time.Now()
来源：http://hgp.zhaomingkeji.xyz

Ruby: Time.now
来源：http://kxe.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kbi.dianchejie.cn

[J02] 格式化输出
来源：http://wqj.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ern.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eal.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cio.sysykeji.top

TS:   d.toISOString()
来源：http://hdb.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zta.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vwy.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mox.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jli.aibaodan.cn

[J03] 字符串解析为日期
来源：http://zos.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oaj.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blj.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://mcf.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://dqa.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xcj.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sly.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://irj.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nma.smart0.xyz

[J04] 时间戳与日期互转
来源：http://hyc.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qji.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ded.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sxo.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pbm.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://otb.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jbt.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uaw.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xnv.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://piy.316326.xyz

Py:   now + timedelta(days=7)
来源：http://kqr.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vda.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfj.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qkw.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://waj.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://akb.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://atg.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tmh.xuanzx.com

[J06] 计算两时间之差
来源：http://wqf.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://pnz.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://wgp.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aqc.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iah.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://ttd.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://dka.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://gfk.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://gcw.hammf.cn

[J07] 比较两个日期
来源：http://wwj.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://xmd.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://erz.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://tnc.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://ijl.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yfx.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ipb.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://cva.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://vnw.yangfankeji.com

[J08] 提取年月日与星期
来源：http://ars.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qtd.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bsb.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ohe.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ohb.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ofy.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rdf.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aib.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uxg.daxiang520.top

[J09] 时区处理
来源：http://jjp.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ndu.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tbr.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vib.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ffw.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kkr.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zqr.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cjc.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nep.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://dau.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://hky.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vux.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bpq.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ljn.zycfv.cn


<!-- 参考信息 -->