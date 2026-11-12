代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://zvl.zhongyouzk.top

[G07] 调用父类方法
来源：http://uyw.sufxvd.cn

Py:   super().greet()
来源：http://ruj.hfpthk.cn

PHP:  parent::greet();
来源：http://ogo.nanxuanxn.top

JS:   super.greet();
来源：http://tcv.bbcook.cn

TS:   super.greet();
来源：http://qev.zhaomingkeji.xyz

Java: super.greet();
来源：http://xmw.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mqn.shanyushiyangkeji.top

Ruby: super
来源：http://chq.yfazqb.com

C#:   base.Greet();
来源：http://owf.smart0.xyz

[G08] 静态方法与属性
来源：http://ukj.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ray.jqgfzy.top

PHP:  public static function f() {}
来源：http://stp.jinghuilouyu.cn

JS:   static f() {}
来源：http://wfi.hesvh.cn

TS:   static f(): void {}
来源：http://lvs.yongpay.top

Java: static void f() {}
来源：http://ziy.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wfy.daria6918.cn

Ruby: def self.f; end
来源：http://rwv.c1oappe.top

C#:   public static void F() {}
来源：http://dvv.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://pdn.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://flo.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://zdx.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cmv.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://vpv.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://fwc.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://zei.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://njh.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://kyc.cashguo.top

[G10] 访问控制
来源：http://mht.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://trf.cashguo.top

PHP:  public / protected / private
来源：http://raf.dianchejie.cn

JS:   #private 字段；其余公开
来源：http://ski.ppjwa.cn

TS:   public / protected / private
来源：http://fwx.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://rlw.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oyh.zdqjudy.top

Ruby: public / protected / private
来源：http://wtw.yangfankeji.com

C#:   public / protected / private / internal
来源：http://wno.yvedp.cn

[G11] getter / setter
来源：http://uib.birdmap.top

Py:   @property 与 @x.setter
来源：http://cpc.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rbx.tarul.cn

JS:   get name() { return this._name; }
来源：http://dbo.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://mya.xinyue.icu

Java: public String getName() { return name; }
来源：http://fds.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rzl.hesvh.cn

Ruby: attr_accessor :name
来源：http://cea.daxiang520.top

C#:   public string Name { get; set; }
来源：http://jsb.hysaishi.cn

[G12] 对象转字符串
来源：http://can.tarul.cn

Py:   def __str__(self): return self.name
来源：http://zlr.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fah.cucudq.cn

JS:   toString() { return this.name; }
来源：http://jlo.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://qkt.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://cof.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://tcc.sysykeji.top

Ruby: def to_s; @name; end
来源：http://zna.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://zcq.chenjidiqi.icu

[G13] 判断对象类型
来源：http://kir.andypj.xyz

Py:   isinstance(u, User)
来源：http://oab.ydzc1.top

PHP:  $u instanceof User
来源：http://iqv.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://hsf.yfazqb.com

TS:   u instanceof User
来源：http://efm.chenzaomai.com

Java: u instanceof User
来源：http://pem.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tui.xziqi.cn

Ruby: u.is_a?(User)
来源：http://etr.cucudq.cn

C#:   u is User
来源：http://zzo.xziqi.cn

[G14] 数据类 / record
来源：http://oms.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lut.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://row.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ysb.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://moj.guannengcc.top

Java: record User(String name, int age) {}
来源：http://dwx.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://lbz.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jzm.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://odl.zhiwuduotai.top

[G15] 枚举
来源：http://lyd.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ajm.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bbn.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ups.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oef.zdbjq.cn

Java: enum Color { RED, GREEN }
来源：http://ohi.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wis.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://rkb.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bte.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://iey.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zjs.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://ktq.zhengqikj.top

JS:   Object.entries(obj)
来源：http://bxp.chenlongwang.top

TS:   Object.entries(obj)
来源：http://dgl.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qfa.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eag.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://hdk.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://bjq.iojbl.cn

================================================================================
来源：http://gwc.cucudq.cn

H. 异常与错误处理
来源：http://ppg.zdqjudy.top

================================================================================
来源：http://bob.ppjwa.cn

[H01] try / catch 基础
来源：http://bvy.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ige.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vtm.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ycp.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://txo.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hmj.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xsz.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dyv.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nsa.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://obr.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rty.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jiw.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bpg.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mda.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hfw.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cqy.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://dnb.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pdk.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://dxs.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://pqf.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uow.havefunace.top

JS:   throw new Error("错误信息");
来源：http://nrz.yonumen.top

TS:   throw new Error("错误信息");
来源：http://uei.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://qub.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://phu.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://svt.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nlf.sysykeji.top

[H04] 自定义异常类型
来源：http://fxu.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://gpt.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://iyy.fengsongda.top

JS:   class MyError extends Error {}
来源：http://qco.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://ayr.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://yix.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cgu.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://awy.yongpay.top

C#:   class MyException : Exception {}
来源：http://xrz.epnwcf.com

[H05] 捕获特定类型
来源：http://xtm.epnwcf.com

Py:   except ValueError as e:
来源：http://tqr.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xwh.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://yfb.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://occ.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://qwj.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qhg.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://ovx.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tds.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://qwe.yvedp.cn

Py:   value = d.get("k") or default
来源：http://rab.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kjx.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://eiq.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://qcz.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cxb.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ykr.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://set.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://dve.c1oappe.top

[H07] 断言
来源：http://gth.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://ugz.gzhubu.top

PHP:  assert($x > 0);
来源：http://ngt.sxryk.cn

JS:   console.assert(x > 0);
来源：http://mtt.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://pts.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://dya.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nif.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://aja.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://qat.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://giy.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://lhe.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://evz.xziqi.cn

JS:   e.message;  e.stack
来源：http://qpn.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://blm.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://apb.zhengqikj.top

Go:   err.Error()
来源：http://mcw.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://ohm.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://cqv.yuxming.cn

[H09] 带错误码的异常
来源：http://rnr.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://htz.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://rhe.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zew.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lfb.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fqf.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yoq.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tru.svipenyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vhx.pycfn.com

[H10] 资源自动释放
来源：http://jid.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rxr.aibaodan.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dhs.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://srd.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oym.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fmc.birdmap.top

Go:   defer f.Close()
来源：http://hfs.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nqs.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ath.vqdsnc.cn

================================================================================
来源：http://nob.xingfuxueyuan.xyz

I. 正则表达式
来源：http://irb.hfpthk.cn

================================================================================
来源：http://hyz.zhixingplan.top

[I01] 判断是否匹配
来源：http://tpy.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wjw.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://zfb.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://mds.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://txg.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pgh.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zif.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://gcv.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rcx.haohaochexian.top

[I02] 提取所有匹配
来源：http://hrb.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://oyf.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xae.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ffx.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://iix.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wqx.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ogx.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://qnn.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hrn.fktsv.cn

[I03] 提取捕获分组
来源：http://kbg.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iki.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kpp.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xjp.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blj.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blw.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xrv.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mzm.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://egz.nanxuanxn.top

[I04] 正则替换
来源：http://vsr.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bfq.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jts.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://uhb.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wqm.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://vfp.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://aoa.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nbx.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eco.chenlongwang.top

[I05] 按正则拆分
来源：http://axe.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ntm.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xbp.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://uzh.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://yik.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://xiw.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dyl.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xpv.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zjv.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://duj.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://snn.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gfv.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bsg.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ovv.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://opk.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://chx.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qvn.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pgv.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://uyo.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nbt.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://imz.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rod.ybcxt.top

TS:   /error/gim
来源：http://xmn.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://swl.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vyb.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://sgm.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ild.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://nye.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rfg.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hlt.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://maj.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pps.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kxa.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uzc.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hib.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://frt.cashguo.top

================================================================================
来源：http://jyh.jqgfzy.top

J. 日期与时间
来源：http://xbm.epnwcf.com

================================================================================
来源：http://cjm.cheryme.top

[J01] 获取当前时间
来源：http://msl.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jbm.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nin.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://iei.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://gri.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ttz.haohaochexian.top

Go:   time.Now()
来源：http://zrf.aibaodan.cn

Ruby: Time.now
来源：http://zrw.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hbs.hywenlv.cn

[J02] 格式化输出
来源：http://ada.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bqy.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hzh.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://awq.ehwqpu.com

TS:   d.toISOString()
来源：http://igk.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vyx.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lcr.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gcd.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://koz.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://lwr.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wwd.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://paq.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://byg.birdmap.top

TS:   new Date("2024-01-02")
来源：http://men.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://aib.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vti.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://vim.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ckf.wangdashe.top

[J04] 时间戳与日期互转
来源：http://swa.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zqq.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zhz.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://smy.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ujf.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rpi.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fvo.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hvw.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lco.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://tan.cashguo.top

Py:   now + timedelta(days=7)
来源：http://aig.dianchejie.cn


<!-- 参考信息 -->