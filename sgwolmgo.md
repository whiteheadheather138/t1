代发 wailian999

Java: interface Shape { double area(); }
来源：http://otk.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://pvc.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rzh.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://srv.nanxuanxn.top

[G10] 访问控制
来源：http://lje.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://vnh.hysaishi.cn

PHP:  public / protected / private
来源：http://nkd.hammf.cn

JS:   #private 字段；其余公开
来源：http://nyu.zdbjq.cn

TS:   public / protected / private
来源：http://gvt.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://pqc.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pvh.guowangkeji.top

Ruby: public / protected / private
来源：http://qga.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://kzo.tianlin.xyz

[G11] getter / setter
来源：http://yup.nwbrower.top

Py:   @property 与 @x.setter
来源：http://lko.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://omt.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://haw.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://ocu.yonumen.top

Java: public String getName() { return name; }
来源：http://uzn.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gcy.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://ogh.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://bma.sxryk.cn

[G12] 对象转字符串
来源：http://qcc.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://cty.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://iqp.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://pch.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://unj.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://aed.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://htg.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://qpp.yongpay.top

C#:   public override string ToString() => Name;
来源：http://nmy.chenlongwang.top

[G13] 判断对象类型
来源：http://myt.jyoumei.cn

Py:   isinstance(u, User)
来源：http://bfw.daria6918.cn

PHP:  $u instanceof User
来源：http://act.guowangkeji.top

JS:   u instanceof User
来源：http://jqz.dashuyun.cn

TS:   u instanceof User
来源：http://vie.cheryme.top

Java: u instanceof User
来源：http://ibz.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://dqq.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://gfn.xuanzx.com

C#:   u is User
来源：http://qzt.jlsjyb.cn

[G14] 数据类 / record
来源：http://qgo.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xtl.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://vgz.tarul.cn

JS:   // 无内置：普通类或对象字面量
来源：http://njk.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://zmo.gzhubu.top

Java: record User(String name, int age) {}
来源：http://bpq.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://bzj.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gwh.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://dhk.haohaochexian.top

[G15] 枚举
来源：http://kag.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nsd.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yoi.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ixr.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jvl.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://pho.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uxz.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://bjg.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hzp.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://pwz.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xdc.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://ajc.cashguo.top

JS:   Object.entries(obj)
来源：http://kfb.cdnleiting.top

TS:   Object.entries(obj)
来源：http://mfk.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://koh.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://yyq.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://cgr.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://gsk.zhaomingkeji.xyz

================================================================================
来源：http://iyj.chenlongwang.top

H. 异常与错误处理
来源：http://kyv.mhx1999.top

================================================================================
来源：http://xdq.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://onu.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nmb.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pxu.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bch.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tss.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uei.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jza.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://psw.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ter.havefunace.top

[H02] finally / ensure 收尾
来源：http://daj.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://buy.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://avw.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bki.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://aed.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qky.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yvn.jqgfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bgj.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rqd.meibo888.top

[H03] 主动抛出异常
来源：http://fwu.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://yda.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mwp.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://mcs.birdmap.top

TS:   throw new Error("错误信息");
来源：http://vuo.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zyp.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hht.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://dow.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://nei.tianlin.xyz

[H04] 自定义异常类型
来源：http://vzu.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://rom.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://kcg.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://rrd.yuxming.cn

TS:   class MyError extends Error {}
来源：http://kqe.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://xrh.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ycu.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://tgn.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://uyq.sjlbkw.cn

[H05] 捕获特定类型
来源：http://iux.yj202588.top

Py:   except ValueError as e:
来源：http://ttk.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cpq.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://rsd.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://gcr.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://vpy.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ptj.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://fif.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vqn.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://vco.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://yee.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://ndm.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://tnu.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://wfm.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eeu.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://mrb.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://yel.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://hza.bjfxy.top

[H07] 断言
来源：http://abn.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://mja.snrcjt.cn

PHP:  assert($x > 0);
来源：http://bbx.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://jue.hammf.cn

TS:   console.assert(x > 0);
来源：http://rbk.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://atd.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gdd.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://gsm.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://xyh.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://oji.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://zpn.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pom.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://xwx.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tmk.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gfv.jqgufenzy.top

Go:   err.Error()
来源：http://nrq.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://qnz.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://cfh.guowangkeji.top

[H09] 带错误码的异常
来源：http://zfc.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://woq.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hdt.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://upa.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vas.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fsx.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nox.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://hly.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zsy.vehdjk.com

[H10] 资源自动释放
来源：http://ywa.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nyg.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oye.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tcp.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dod.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gsz.xinyue.icu

Go:   defer f.Close()
来源：http://rkb.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yda.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://npa.haohaochexian.top

================================================================================
来源：http://lnj.yvedp.cn

I. 正则表达式
来源：http://gab.jqgfzy.top

================================================================================
来源：http://fwc.dashuyun.cn

[I01] 判断是否匹配
来源：http://fqq.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jxg.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://buq.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://pwd.havefunace.top

TS:   /\d+/.test(s)
来源：http://ghp.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mqy.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ong.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://xxp.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qlm.svipenyu.cn

[I02] 提取所有匹配
来源：http://pha.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://vgt.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://npk.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dmv.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://jvs.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jwb.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ynn.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://arl.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kxe.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://jta.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ftn.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aqa.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qgf.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ebr.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hwo.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ksi.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nsg.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hfh.hywenlv.cn

[I04] 正则替换
来源：http://uow.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://plk.yj202588.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://syb.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pvn.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://ldf.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://fbj.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://adh.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rhv.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hnm.nanxuanxn.top

[I05] 按正则拆分
来源：http://xvo.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tat.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dwc.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://ihr.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://iow.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://tup.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wnr.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://arw.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uid.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pny.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nlk.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://suw.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxm.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rgf.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ziy.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://klz.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hgz.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://asf.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://gqk.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sbb.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qpu.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://clj.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://kjb.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nfe.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gtg.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://vpj.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mfu.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://dbu.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dgq.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uwa.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvf.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lfm.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://blb.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qkm.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jdl.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rcr.ehwqpu.com

================================================================================
来源：http://lcu.wangdashe.top

J. 日期与时间
来源：http://psp.9152youxi.cn

================================================================================
来源：http://gzz.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://thm.cheryme.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://acu.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vib.pycfn.com

JS:   new Date();  Date.now()
来源：http://hsh.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://uxz.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://jtt.fzhhl.top

Go:   time.Now()
来源：http://uoz.ydjk.org.cn

Ruby: Time.now
来源：http://hfy.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://epp.gogol.net.cn

[J02] 格式化输出
来源：http://evt.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jpr.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ecf.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ypg.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://mel.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zmm.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ihl.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fge.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fsf.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://aba.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://myf.cheryme.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rbd.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://jvn.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://aze.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://ghq.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lmy.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://opw.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kpb.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://zbd.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://msv.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jcq.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ogt.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mdy.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zex.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yvh.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ske.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oxp.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://zvi.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://icf.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lia.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jsc.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvh.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://xim.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wcb.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://tsy.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bur.pycfn.com

[J06] 计算两时间之差
来源：http://xej.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://cmv.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://kyh.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vbp.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ujd.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jlg.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://qrt.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://ewu.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://ovl.yvedp.cn

[J07] 比较两个日期
来源：http://xhv.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://mst.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ueq.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sbs.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://iti.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kfi.jqgfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esk.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://mry.316326.xyz


<!-- 参考信息 -->