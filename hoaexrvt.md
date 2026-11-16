代发 wailian999

[G06] 重写方法
来源：http://lsl.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://jxj.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xej.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://sca.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://ygd.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://tem.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gzb.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://ekn.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://mxw.jyoumei.cn

[G07] 调用父类方法
来源：http://taj.0kj1m.cn

Py:   super().greet()
来源：http://kru.ybcxt.top

PHP:  parent::greet();
来源：http://etx.zdqjudy.top

JS:   super.greet();
来源：http://fob.zhixingplan.top

TS:   super.greet();
来源：http://jrr.epnwcf.com

Java: super.greet();
来源：http://mjb.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oyd.yueranfly.top

Ruby: super
来源：http://qdt.zhoulong.xyz

C#:   base.Greet();
来源：http://hun.gzhubu.top

[G08] 静态方法与属性
来源：http://wpc.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://acs.vehdjk.com

PHP:  public static function f() {}
来源：http://jrc.sufxvd.cn

JS:   static f() {}
来源：http://ngu.jianghu66.top

TS:   static f(): void {}
来源：http://ped.xuanzx.com

Java: static void f() {}
来源：http://wyz.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://csr.sweek.top

Ruby: def self.f; end
来源：http://hvo.cucudq.cn

C#:   public static void F() {}
来源：http://cyg.fzhhl.top

[G09] 接口 / 抽象类
来源：http://ovj.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://yjw.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://uwv.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lqk.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://ozg.gzhubu.top

Java: interface Shape { double area(); }
来源：http://cvz.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://lho.yj202588.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hvi.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://vmc.nanxuanxn.top

[G10] 访问控制
来源：http://ffw.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://hmc.9152youxi.cn

PHP:  public / protected / private
来源：http://qze.fengsongda.top

JS:   #private 字段；其余公开
来源：http://xiv.hnxiangtu.top

TS:   public / protected / private
来源：http://fyq.birdmap.top

Java: public / protected / private / 默认包级
来源：http://rxj.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dfi.yfazqb.com

Ruby: public / protected / private
来源：http://zrt.mhx1999.top

C#:   public / protected / private / internal
来源：http://fol.jinqigfzy.top

[G11] getter / setter
来源：http://yyd.ybcxt.top

Py:   @property 与 @x.setter
来源：http://aio.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://okt.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://tdv.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://dnm.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://wpv.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://pnc.hnqzz.top

Ruby: attr_accessor :name
来源：http://dbt.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://ing.chenjidiqi.icu

[G12] 对象转字符串
来源：http://krt.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://osu.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mpb.daxiang520.top

JS:   toString() { return this.name; }
来源：http://jcc.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://pvd.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://ssg.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mxt.yfazqb.com

Ruby: def to_s; @name; end
来源：http://ibt.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://oxp.hammf.cn

[G13] 判断对象类型
来源：http://tky.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://hfd.9152youxi.cn

PHP:  $u instanceof User
来源：http://lqi.zhijiandao.cn

JS:   u instanceof User
来源：http://lja.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://oqn.hfpthk.cn

Java: u instanceof User
来源：http://bjt.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ycp.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://kfh.52xcode.cn

C#:   u is User
来源：http://asl.yvedp.cn

[G14] 数据类 / record
来源：http://xof.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kxu.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://wcz.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rrp.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://kwa.ybcxt.top

Java: record User(String name, int age) {}
来源：http://vnv.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://dwk.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qhb.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://psf.iojbl.cn

[G15] 枚举
来源：http://xgb.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ztb.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gkf.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kzv.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qxo.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://eud.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://czc.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://uko.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zkk.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://oic.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mgx.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://ttk.sysykeji.top

JS:   Object.entries(obj)
来源：http://yao.tianlin.xyz

TS:   Object.entries(obj)
来源：http://nkw.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vss.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://zzo.smart0.xyz

Ruby: obj.instance_variables
来源：http://isn.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://dhu.nanxinkj.top

================================================================================
来源：http://mvk.ivvv.top

H. 异常与错误处理
来源：http://fqx.zhiwuduotai.top

================================================================================
来源：http://hag.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://ewr.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dzf.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mxi.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jcl.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gye.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vmn.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oys.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nzx.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iuc.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://nks.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gfp.ppjwa.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vsk.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tas.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://wic.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://bxr.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qtw.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://was.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kyj.bbcook.cn

[H03] 主动抛出异常
来源：http://hcu.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://snf.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mpt.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://yau.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://eny.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hun.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sle.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pkf.hammf.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mzb.epnwcf.com

[H04] 自定义异常类型
来源：http://fzf.yongpay.top

Py:   class MyError(Exception): pass
来源：http://dog.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://hlq.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://krn.sxryk.cn

TS:   class MyError extends Error {}
来源：http://ulb.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://bwq.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://avg.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://zzf.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://ums.gogol.net.cn

[H05] 捕获特定类型
来源：http://pla.jiagoushi.top

Py:   except ValueError as e:
来源：http://syb.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zbq.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://jvc.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://xpk.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://thq.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dwc.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://ale.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mri.vehdjk.com

[H06] 可选值 / 空值安全访问
来源：http://kzm.xziqi.cn

Py:   value = d.get("k") or default
来源：http://gmp.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xtl.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://yqq.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://duh.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ktz.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xyt.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://nal.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://kjx.ehwqpu.com

[H07] 断言
来源：http://vwd.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://cfd.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://zhu.cheryme.top

JS:   console.assert(x > 0);
来源：http://ajq.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://bcv.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://uqo.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gqi.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://sjz.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://flb.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://nfg.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://nsx.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qla.iojbl.cn

JS:   e.message;  e.stack
来源：http://gce.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wme.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zmg.sysykeji.top

Go:   err.Error()
来源：http://tho.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://fgu.kuanghao11.cn

C#:   e.Message;  e.StackTrace
来源：http://wkx.zdqjudy.top

[H09] 带错误码的异常
来源：http://cak.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cad.shzxlz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vpt.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xbq.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ynm.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yys.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://onl.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://cjl.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://zeo.uphjek.com

[H10] 资源自动释放
来源：http://tvo.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fvy.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nkw.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qtz.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://her.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mul.vqdsnc.cn

Go:   defer f.Close()
来源：http://ddd.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rfk.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://itk.wangdashe.top

================================================================================
来源：http://auw.pengpengdd.cyou

I. 正则表达式
来源：http://vad.andypj.xyz

================================================================================
来源：http://zdh.aibaodan.cn

[I01] 判断是否匹配
来源：http://oih.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://opz.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://mxd.pycfn.com

JS:   /\d+/.test(s)
来源：http://mno.zycfv.cn

TS:   /\d+/.test(s)
来源：http://zky.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ewc.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://liu.havefunace.top

Ruby: s.match?(/\d+/)
来源：http://sgx.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lmt.sxryk.cn

[I02] 提取所有匹配
来源：http://cbm.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://yjr.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kzi.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jrw.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://nkl.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yoq.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://msh.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://xpj.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tss.cdnleiting.top

[I03] 提取捕获分组
来源：http://gxz.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dzy.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sel.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ygi.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fvg.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qbc.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://igo.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tgg.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fdb.shanyushiyangkeji.top

[I04] 正则替换
来源：http://ytn.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iwo.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yde.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gjo.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://dmb.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://roc.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ywb.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vun.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fqf.yj202588.top

[I05] 按正则拆分
来源：http://eev.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://zra.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://keg.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://isp.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://afx.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://bqk.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zov.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fxv.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kvg.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ipc.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xew.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tal.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bln.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vri.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://znq.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kim.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yqo.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kji.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://ytl.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qix.sufxvd.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wnz.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://frt.iojbl.cn

TS:   /error/gim
来源：http://wlq.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zkw.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jps.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://ydr.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wvr.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://nbm.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ryp.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eju.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zgw.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zsi.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fqh.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sfq.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ebx.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://afk.yvedp.cn

================================================================================
来源：http://gxn.ehwqpu.com

J. 日期与时间
来源：http://zis.xinyue.icu

================================================================================
来源：http://xzq.0kj1m.cn

[J01] 获取当前时间
来源：http://jbn.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bec.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dre.shuidangran.top

JS:   new Date();  Date.now()
来源：http://sqs.yj202588.top

TS:   new Date();  Date.now()
来源：http://iky.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oqo.hywenlv.cn

Go:   time.Now()
来源：http://dtj.pengpengdd.cyou

Ruby: Time.now
来源：http://xba.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ven.yongpay.top

[J02] 格式化输出
来源：http://iba.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zyw.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://osv.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hty.zhoulong.xyz

TS:   d.toISOString()
来源：http://try.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qgh.jianghu66.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zgq.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rmv.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hco.guowangkeji.top

[J03] 字符串解析为日期
来源：http://qcf.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fdj.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cgy.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://jnl.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://ycl.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://qzw.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tef.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://jrx.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ztn.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://xmf.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hvx.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://len.fktsv.cn


<!-- 参考信息 -->