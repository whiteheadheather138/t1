代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://avy.vehdjk.com

[G07] 调用父类方法
来源：http://goe.wangdashe.top

Py:   super().greet()
来源：http://xal.hammf.cn

PHP:  parent::greet();
来源：http://lkd.fktsv.cn

JS:   super.greet();
来源：http://wza.hammf.cn

TS:   super.greet();
来源：http://nav.hongshengwenyu.top

Java: super.greet();
来源：http://giu.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oww.birdmap.top

Ruby: super
来源：http://nwk.xinyue.icu

C#:   base.Greet();
来源：http://cgc.hfpthk.cn

[G08] 静态方法与属性
来源：http://rcq.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lnt.sysykeji.top

PHP:  public static function f() {}
来源：http://hmq.fehbvm.com

JS:   static f() {}
来源：http://xap.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://zmu.shangyingyoupin.top

Java: static void f() {}
来源：http://rzc.guowangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hws.ctjpmb.com

Ruby: def self.f; end
来源：http://laa.jyoumei.cn

C#:   public static void F() {}
来源：http://fna.fzhhl.top

[G09] 接口 / 抽象类
来源：http://ura.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://jmw.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://sss.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://unh.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://pir.sxryk.cn

Java: interface Shape { double area(); }
来源：http://sun.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://cmj.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ibn.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://vpi.snrcjt.cn

[G10] 访问控制
来源：http://icl.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://pgr.jinqigfzy.top

PHP:  public / protected / private
来源：http://qql.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://vtl.fzhhl.top

TS:   public / protected / private
来源：http://dfo.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://tki.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jkt.xziqi.cn

Ruby: public / protected / private
来源：http://mxl.cashguo.top

C#:   public / protected / private / internal
来源：http://iwq.dianchejie.cn

[G11] getter / setter
来源：http://zjh.52xcode.cn

Py:   @property 与 @x.setter
来源：http://aff.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vys.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://pbx.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://jbh.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://bgl.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://spu.xylfe.cn

Ruby: attr_accessor :name
来源：http://vfg.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://tvd.jlsjyb.cn

[G12] 对象转字符串
来源：http://edc.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://aec.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ety.ctjpmb.com

JS:   toString() { return this.name; }
来源：http://khq.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://qbc.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://xea.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ejp.c1oappe.top

Ruby: def to_s; @name; end
来源：http://vxm.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://jzy.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://fzl.ydzc1.top

Py:   isinstance(u, User)
来源：http://lkq.kuanghao11.cn

PHP:  $u instanceof User
来源：http://pqe.yj202588.top

JS:   u instanceof User
来源：http://nil.ehwqpu.com

TS:   u instanceof User
来源：http://ykm.dashuyun.cn

Java: u instanceof User
来源：http://xpc.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iot.ydzc1.top

Ruby: u.is_a?(User)
来源：http://pli.c1oappe.top

C#:   u is User
来源：http://ino.havefunace.top

[G14] 数据类 / record
来源：http://fpo.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://krp.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://vwg.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://odg.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://sje.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://bqy.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://nqi.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://esq.yj20258888.top

C#:   record User(string Name, int Age);
来源：http://lgn.hongshengwenyu.top

[G15] 枚举
来源：http://oiz.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gjo.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hou.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zyv.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zvc.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://fho.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vkk.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://qsk.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nre.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://nkw.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gbc.fengsongda.top

PHP:  get_object_vars($obj);
来源：http://rvc.zhixingplan.top

JS:   Object.entries(obj)
来源：http://cxo.tanke756.top

TS:   Object.entries(obj)
来源：http://yix.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cug.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://afa.zhengqikj.top

Ruby: obj.instance_variables
来源：http://xzd.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://jiy.cashguo.top

================================================================================
来源：http://fle.birdmap.top

H. 异常与错误处理
来源：http://lzv.jqgfzy.top

================================================================================
来源：http://sfd.hywenlv.cn

[H01] try / catch 基础
来源：http://wgg.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jth.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jti.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zop.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://imd.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://otp.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hot.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hsz.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zfn.jianghu66.top

[H02] finally / ensure 收尾
来源：http://vkh.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://bqt.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hng.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ykt.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bst.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://skf.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hcz.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ujh.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yxo.zhoulong.xyz

[H03] 主动抛出异常
来源：http://bxb.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://plt.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jwq.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://afs.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://xzq.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hro.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qza.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://emz.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://dqx.cdnleiting.top

[H04] 自定义异常类型
来源：http://iks.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://twm.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://any.wangdashe.top

JS:   class MyError extends Error {}
来源：http://kpb.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://ybg.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://jgn.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xqq.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://pbr.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://ghx.bbcook.cn

[H05] 捕获特定类型
来源：http://sqx.dianchejie.cn

Py:   except ValueError as e:
来源：http://clv.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pwn.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://muw.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://ckw.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://tge.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fno.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://gmf.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ufx.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://wtl.cheryme.top

Py:   value = d.get("k") or default
来源：http://ogk.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://mtm.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://nvb.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fyf.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wrh.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cng.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://nin.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://psb.zhoulong.xyz

[H07] 断言
来源：http://gou.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://crx.zhixingplan.top

PHP:  assert($x > 0);
来源：http://bra.hammf.cn

JS:   console.assert(x > 0);
来源：http://eay.epnwcf.com

TS:   console.assert(x > 0);
来源：http://zwj.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://fna.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cdz.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jjq.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://bpt.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://pjl.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://qev.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zpc.ydzc1.top

JS:   e.message;  e.stack
来源：http://lvg.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kcu.jqgfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ssq.chenlongwang.top

Go:   err.Error()
来源：http://ncx.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://hcq.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://rks.snrcjt.cn

[H09] 带错误码的异常
来源：http://wje.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ycc.haohaochexian.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sle.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bkx.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zek.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://muo.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ysc.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://uyz.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kre.hnxiangtu.top

[H10] 资源自动释放
来源：http://vtj.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://umo.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lcc.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cwy.jinqigfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jsk.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ahq.zhengqikj.top

Go:   defer f.Close()
来源：http://jef.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pji.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jnw.hcnkem.com

================================================================================
来源：http://xtk.nanxinkj.top

I. 正则表达式
来源：http://upl.52xcode.cn

================================================================================
来源：http://qrv.haohaochexian.top

[I01] 判断是否匹配
来源：http://zgo.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fau.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://khu.havefunace.top

JS:   /\d+/.test(s)
来源：http://xwm.zycfv.cn

TS:   /\d+/.test(s)
来源：http://pxm.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lzs.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zeq.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://zha.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://npq.hcnkem.com

[I02] 提取所有匹配
来源：http://nxx.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://uwe.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cqr.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ktj.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://thq.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lus.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://azl.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://rlw.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jqq.yfazqb.com

[I03] 提取捕获分组
来源：http://kcl.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wnc.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://onp.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lil.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qmj.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mee.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tic.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qtr.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jal.kuanghao11.cn

[I04] 正则替换
来源：http://cim.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qon.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mlm.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://ijr.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://pbi.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://suu.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eyh.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mwn.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cdb.jlsjyb.cn

[I05] 按正则拆分
来源：http://gls.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vkk.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kuq.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://quy.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://tdu.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://eun.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gke.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fdh.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kjd.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://frs.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://znz.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://avd.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sbh.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pbk.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ixh.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ivi.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bhx.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://egm.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://fyt.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kkr.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pyg.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wsp.bjfxy.top

TS:   /error/gim
来源：http://qza.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jnc.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gyz.uphjek.com

Ruby: s.scan(/error/i)
来源：http://kns.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gak.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://rai.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pvl.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yoa.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://slk.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bnm.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://mmd.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pkr.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jaa.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hih.epnwcf.com

================================================================================
来源：http://mvb.cashguo.top

J. 日期与时间
来源：http://ing.shzxlz.cn

================================================================================
来源：http://uee.tanke756.top

[J01] 获取当前时间
来源：http://yyg.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nlw.zdqjudy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eve.fengsongda.top

JS:   new Date();  Date.now()
来源：http://hni.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://odf.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rtk.0kj1m.cn

Go:   time.Now()
来源：http://hcv.guowangkeji.top

Ruby: Time.now
来源：http://bog.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://byt.tian-w.cn

[J02] 格式化输出
来源：http://lak.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mfq.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://szt.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hqy.hammf.cn

TS:   d.toISOString()
来源：http://pha.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://evq.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rmt.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tld.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lgm.tianlin.xyz

[J03] 字符串解析为日期
来源：http://nxs.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wfl.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mil.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://nse.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://ihc.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://mug.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://crc.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://zgq.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ttv.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://yct.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://neo.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cbd.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://trj.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://coo.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cwp.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gem.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qzp.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bmj.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://ldn.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://xza.sufxvd.cn


<!-- 参考信息 -->