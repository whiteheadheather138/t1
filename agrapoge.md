代发 wailian999

Java: class Admin extends User {}
来源：http://yet.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wgw.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://mul.jinqigufen.top

C#:   class Admin : User {}
来源：http://fqq.wangshuangyany.cn

[G06] 重写方法
来源：http://ehg.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://wzk.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://set.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://agn.jiagoushi.top

TS:   greet(): string { return "admin"; }
来源：http://qol.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://gvy.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ogq.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://wkr.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://ylv.fehbvm.com

[G07] 调用父类方法
来源：http://dzt.zhongyouzk.top

Py:   super().greet()
来源：http://umv.fehbvm.com

PHP:  parent::greet();
来源：http://qaz.daria6918.cn

JS:   super.greet();
来源：http://ouj.gzhubu.top

TS:   super.greet();
来源：http://rhk.ydzc1.top

Java: super.greet();
来源：http://yqg.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qko.iojbl.cn

Ruby: super
来源：http://mef.xylfe.cn

C#:   base.Greet();
来源：http://xgq.nanxinkj.top

[G08] 静态方法与属性
来源：http://haf.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://slk.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://yrp.zhijiandao.cn

JS:   static f() {}
来源：http://rcf.zycfv.cn

TS:   static f(): void {}
来源：http://dty.epnwcf.com

Java: static void f() {}
来源：http://ncj.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tww.jqgufenzy.top

Ruby: def self.f; end
来源：http://egi.gotoacloud.top

C#:   public static void F() {}
来源：http://bap.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://rmf.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://mvt.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jpg.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lsw.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://occ.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://vqh.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://mnn.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kob.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://qfd.uphjek.com

[G10] 访问控制
来源：http://ohe.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://mgv.zhijiandao.cn

PHP:  public / protected / private
来源：http://prb.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://tpu.ydjk.org.cn

TS:   public / protected / private
来源：http://boj.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://iot.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vqw.wangshuangyany.cn

Ruby: public / protected / private
来源：http://osg.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://oyw.uphjek.com

[G11] getter / setter
来源：http://qbb.hcnkem.com

Py:   @property 与 @x.setter
来源：http://uum.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://vxj.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://dkx.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://oyy.yj20258.top

Java: public String getName() { return name; }
来源：http://kxq.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ymy.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://gco.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://dvb.yvedp.cn

[G12] 对象转字符串
来源：http://vyr.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://gix.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zug.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://fel.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://rxz.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://cyn.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lpm.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://fvx.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://kip.cashguo.top

[G13] 判断对象类型
来源：http://jsp.hcnkem.com

Py:   isinstance(u, User)
来源：http://ovr.gogol.net.cn

PHP:  $u instanceof User
来源：http://ldi.9152youxi.cn

JS:   u instanceof User
来源：http://exb.ppjwa.cn

TS:   u instanceof User
来源：http://vey.fanxiaobao.xyz

Java: u instanceof User
来源：http://gwo.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lkh.meibo888.top

Ruby: u.is_a?(User)
来源：http://kkw.fktsv.cn

C#:   u is User
来源：http://wob.dashuyun.cn

[G14] 数据类 / record
来源：http://khm.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://owq.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://pva.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://ibs.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://cvs.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://jai.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://rsr.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ogw.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://kil.nanxinkj.top

[G15] 枚举
来源：http://pib.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pfw.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hyp.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bbd.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://efx.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://ruw.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xwe.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://zxo.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iri.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://wnt.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sxs.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://ino.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://hdm.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://kyd.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kwe.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xcw.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://hgp.ctjpmb.com

C#:   // 用反射或 System.Text.Json
来源：http://uzj.feifeiyinyue.top

================================================================================
来源：http://pip.jqgufenzy.top

H. 异常与错误处理
来源：http://mjx.cqqwz.cn

================================================================================
来源：http://gzf.gogol.net.cn

[H01] try / catch 基础
来源：http://tkx.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jaz.jinghuilouyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qsb.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cin.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xjo.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pcf.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fih.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ebe.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bfs.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://tgu.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pwy.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ysd.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ukj.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ngw.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yxi.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hjq.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tts.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tez.yangfankeji.com

[H03] 主动抛出异常
来源：http://duh.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://pxt.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ein.zhoulong.xyz

JS:   throw new Error("错误信息");
来源：http://cpm.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://tyh.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mny.chenzaomai.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://glx.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://enz.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://kxp.sysykeji.top

[H04] 自定义异常类型
来源：http://vco.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://lka.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://fbz.cashguo.top

JS:   class MyError extends Error {}
来源：http://qev.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://brg.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://jih.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nku.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://kqq.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://dzz.tianlin.xyz

[H05] 捕获特定类型
来源：http://kqn.yuxming.cn

Py:   except ValueError as e:
来源：http://wge.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wmx.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://anb.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://alq.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://mpf.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kxm.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://pcm.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sfa.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://coi.pycfn.com

Py:   value = d.get("k") or default
来源：http://lnt.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://squ.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wrs.zhengqikj.top

TS:   obj?.a?.b;  d ?? default
来源：http://zsp.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nta.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pks.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://mce.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://iqd.guannengcc.top

[H07] 断言
来源：http://pek.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://ped.yueranfly.top

PHP:  assert($x > 0);
来源：http://usp.cheryme.top

JS:   console.assert(x > 0);
来源：http://kah.meibo888.top

TS:   console.assert(x > 0);
来源：http://evv.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://fmn.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://phw.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://gxv.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://mmu.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://jxt.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://xuw.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ktz.uphjek.com

JS:   e.message;  e.stack
来源：http://zvi.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xtx.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hfn.yj20258.top

Go:   err.Error()
来源：http://zda.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://mqg.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://fqz.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://ime.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qxz.yj20258888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bbs.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mkb.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xkh.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qdk.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wbv.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://igi.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gzf.yuanzhike.top

[H10] 资源自动释放
来源：http://ikf.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://szz.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ycv.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nii.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pot.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fkp.cheryme.top

Go:   defer f.Close()
来源：http://axs.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rqw.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ntg.iojbl.cn

================================================================================
来源：http://uis.vqdsnc.cn

I. 正则表达式
来源：http://bgd.tanke756.top

================================================================================
来源：http://obk.chenlongwang.top

[I01] 判断是否匹配
来源：http://zyt.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cas.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gjz.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://gay.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://sja.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rsr.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vgk.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://nuc.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dkx.redwolf501.top

[I02] 提取所有匹配
来源：http://ykx.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://kza.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://acl.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rxn.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://uqw.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mai.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gbo.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://zqu.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ngn.tian-w.cn

[I03] 提取捕获分组
来源：http://lvg.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zjk.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uqa.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hri.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jwk.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pqb.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kak.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jrg.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rnr.yj202588.top

[I04] 正则替换
来源：http://igi.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cfp.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tcf.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cdn.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://kgk.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://ers.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gal.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ylk.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ikb.yj20258888.top

[I05] 按正则拆分
来源：http://nfd.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nqh.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vqk.yvedp.cn

JS:   s.split(/\s*,\s*/)
来源：http://qmc.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://erj.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://sek.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bbb.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://eop.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zae.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://suw.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bao.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oah.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wba.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://syo.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ozl.xuetiantiany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://esd.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pqa.wangdashe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bic.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://rid.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zca.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vmt.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://esp.bjfxy.top

TS:   /error/gim
来源：http://mzt.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jnd.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xce.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://spx.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rsf.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://lxu.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wyl.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://svi.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvr.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uke.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://whd.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vme.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aha.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ixe.bjfxy.top

================================================================================
来源：http://cub.jiagoushi.top

J. 日期与时间
来源：http://zeb.gzhubu.top

================================================================================
来源：http://wcf.c1oappe.top

[J01] 获取当前时间
来源：http://bfo.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mid.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pug.iojbl.cn

JS:   new Date();  Date.now()
来源：http://ofk.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://lld.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://klv.daria6918.cn

Go:   time.Now()
来源：http://ocv.jyoumei.cn

Ruby: Time.now
来源：http://psq.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ejd.havefunace.top

[J02] 格式化输出
来源：http://isn.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fue.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oij.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tnw.tianlin.xyz

TS:   d.toISOString()
来源：http://nwj.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eku.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tin.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pto.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lln.cqqwz.cn

[J03] 字符串解析为日期
来源：http://aon.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mmf.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mof.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://qdz.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://vzr.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://sfy.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ada.guowangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://vfm.yueranfly.top


<!-- 参考信息 -->