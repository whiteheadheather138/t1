代发 wailian999

PHP:  public static function f() {}
来源：http://jjg.hfpthk.cn

JS:   static f() {}
来源：http://gms.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://iuw.gotoacloud.top

Java: static void f() {}
来源：http://udl.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://noj.jianghu66.top

Ruby: def self.f; end
来源：http://dwk.fehbvm.com

C#:   public static void F() {}
来源：http://ipj.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://hbt.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://bun.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pvy.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bwy.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://vkl.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://xjz.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://bgq.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tbx.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://scs.mhx1999.top

[G10] 访问控制
来源：http://tih.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ffb.gzhubu.top

PHP:  public / protected / private
来源：http://yhf.sweek.top

JS:   #private 字段；其余公开
来源：http://fcj.ydjk.org.cn

TS:   public / protected / private
来源：http://xgw.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://tgh.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hcu.daria6918.cn

Ruby: public / protected / private
来源：http://ftq.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://fnf.ehwqpu.com

[G11] getter / setter
来源：http://vom.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://tix.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hnm.zycfv.cn

JS:   get name() { return this._name; }
来源：http://fsb.jinqigfzy.top

TS:   get name(): string { return this._name; }
来源：http://avn.yj20258.top

Java: public String getName() { return name; }
来源：http://jpg.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lwr.daria6918.cn

Ruby: attr_accessor :name
来源：http://eci.birdmap.top

C#:   public string Name { get; set; }
来源：http://zfr.nanxuanxn.top

[G12] 对象转字符串
来源：http://uan.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://jgf.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jtp.tarul.cn

JS:   toString() { return this.name; }
来源：http://umg.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://ifn.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://ako.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://umd.yonumen.top

Ruby: def to_s; @name; end
来源：http://blc.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://vdk.hfpthk.cn

[G13] 判断对象类型
来源：http://ouc.shuidangran.top

Py:   isinstance(u, User)
来源：http://qln.guowangkeji.top

PHP:  $u instanceof User
来源：http://mnb.xuanzx.com

JS:   u instanceof User
来源：http://rpd.mhx1999.top

TS:   u instanceof User
来源：http://xuf.ivvv.top

Java: u instanceof User
来源：http://izq.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xbw.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://lnd.yvedp.cn

C#:   u is User
来源：http://qjg.316326.xyz

[G14] 数据类 / record
来源：http://ipe.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uzu.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://xtn.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://jnt.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://pre.xinyue.icu

Java: record User(String name, int age) {}
来源：http://inf.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://zwt.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jsi.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://usw.uphjek.com

[G15] 枚举
来源：http://wez.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mlf.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://khf.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tnq.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://txg.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://tcp.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pkl.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://vws.xingfuxueyuan.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://egc.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://uch.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vev.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://emm.xziqi.cn

JS:   Object.entries(obj)
来源：http://utu.yueranfly.top

TS:   Object.entries(obj)
来源：http://jbi.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pej.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ijh.0kj1m.cn

Ruby: obj.instance_variables
来源：http://ond.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://lei.chenzaomai.com

================================================================================
来源：http://hfs.zycfv.cn

H. 异常与错误处理
来源：http://xsz.ctjpmb.com

================================================================================
来源：http://akm.fktsv.cn

[H01] try / catch 基础
来源：http://ybc.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eoe.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rux.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oqi.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dxa.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gdq.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hkd.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lng.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hdm.mhx1999.top

[H02] finally / ensure 收尾
来源：http://iaq.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qdi.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lsm.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ebd.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://puy.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://okx.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nsr.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pye.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yec.zhoulong.xyz

[H03] 主动抛出异常
来源：http://uif.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://xsd.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xdu.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://bpo.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://sny.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jpq.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cli.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wzr.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://onn.andypj.xyz

[H04] 自定义异常类型
来源：http://iii.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://dsd.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://yan.yj20258888.top

JS:   class MyError extends Error {}
来源：http://iwf.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://jdm.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://xhz.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nsn.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://hog.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://agm.jianghu66.top

[H05] 捕获特定类型
来源：http://cdk.yfazqb.com

Py:   except ValueError as e:
来源：http://qev.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ntv.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://bja.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://xki.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://xti.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dbx.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://cau.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yfh.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://sbi.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://pqz.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://uik.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cpw.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wmx.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://osr.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pwz.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://djl.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://bkk.wangdashe.top

[H07] 断言
来源：http://bgh.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://ubd.dashuyun.cn

PHP:  assert($x > 0);
来源：http://qwl.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://tda.c1oappe.top

TS:   console.assert(x > 0);
来源：http://puc.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://kkq.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://igh.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vih.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://upo.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://fbj.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://cdc.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://knh.svipenyu.cn

JS:   e.message;  e.stack
来源：http://rts.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fxa.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://gwv.zycfv.cn

Go:   err.Error()
来源：http://unx.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://qnu.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://qag.guowangkeji.top

[H09] 带错误码的异常
来源：http://lzs.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wot.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sam.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hri.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://akx.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zvd.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nlr.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://yqb.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vik.havefunace.top

[H10] 资源自动释放
来源：http://hau.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mad.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ypa.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lfi.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jjb.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://owc.xinyue.icu

Go:   defer f.Close()
来源：http://twp.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xsb.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ewy.uphjek.com

================================================================================
来源：http://aez.tarul.cn

I. 正则表达式
来源：http://abt.sufxvd.cn

================================================================================
来源：http://aen.52xcode.cn

[I01] 判断是否匹配
来源：http://yni.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ldk.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://lmp.316326.xyz

JS:   /\d+/.test(s)
来源：http://sdc.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://qqj.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gmi.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nvc.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://ygq.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zza.fehbvm.com

[I02] 提取所有匹配
来源：http://bcr.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://lqk.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://neo.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://swv.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://ejf.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uoc.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://exg.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://aoa.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qjx.daxiang520.top

[I03] 提取捕获分组
来源：http://zka.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mqr.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vxh.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iwt.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://twg.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kfp.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yqx.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cqu.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://omz.hesvh.cn

[I04] 正则替换
来源：http://yyi.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://fcg.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qlv.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://frs.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://sov.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://jte.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://gxo.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zzv.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://spt.cdnleiting.top

[I05] 按正则拆分
来源：http://xzy.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ots.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pty.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://hel.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://ucb.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://ayc.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://btk.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://wss.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zyn.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://won.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rcb.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nfi.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kle.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fwv.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tft.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://psi.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lqy.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eqa.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://fgd.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xgz.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gth.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ufm.guannengcc.top

TS:   /error/gim
来源：http://bky.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dll.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iju.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://qbh.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ixq.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://lbn.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ipq.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bpf.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qbc.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pdk.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://naa.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qvx.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qbj.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://szj.tian-w.cn

================================================================================
来源：http://nmf.kuanghao11.cn

J. 日期与时间
来源：http://odp.gzhubu.top

================================================================================
来源：http://bii.hcnkem.com

[J01] 获取当前时间
来源：http://ied.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fnv.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gup.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://uhd.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://kxn.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mto.feifeiyinyue.top

Go:   time.Now()
来源：http://cac.sufxvd.cn

Ruby: Time.now
来源：http://fwr.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zrm.hywenlv.cn

[J02] 格式化输出
来源：http://hvs.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ekl.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uym.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ctz.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://yay.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hkt.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wxe.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qco.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://flg.yongpay.top

[J03] 字符串解析为日期
来源：http://ilb.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cfh.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yzv.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://baf.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://tqa.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zsj.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wsd.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://rqg.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://stj.xylfe.cn

[J04] 时间戳与日期互转
来源：http://ltg.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zyw.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gii.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ktq.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cxc.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qrs.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xrr.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gui.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ctr.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://eil.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://phx.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zzc.52xcode.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rcb.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ppu.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://tou.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dzx.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://mtk.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mzh.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://cdh.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://yth.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://bsw.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qse.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ohi.redwolf501.top


<!-- 参考信息 -->