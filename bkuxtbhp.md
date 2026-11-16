代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://bez.wangshuangyany.cn

[G07] 调用父类方法
来源：http://shu.daria6918.cn

Py:   super().greet()
来源：http://uym.sweek.top

PHP:  parent::greet();
来源：http://pqf.hysaishi.cn

JS:   super.greet();
来源：http://okx.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://adj.xylfe.cn

Java: super.greet();
来源：http://wre.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hvr.chenlongwang.top

Ruby: super
来源：http://oms.uphjek.com

C#:   base.Greet();
来源：http://gon.fktsv.cn

[G08] 静态方法与属性
来源：http://pkm.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pjy.jinqigfzy.top

PHP:  public static function f() {}
来源：http://njn.guowangkeji.top

JS:   static f() {}
来源：http://onk.316326.xyz

TS:   static f(): void {}
来源：http://dbp.cucudq.cn

Java: static void f() {}
来源：http://mjm.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://njb.zhongyouzk.top

Ruby: def self.f; end
来源：http://hjd.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://tms.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://jec.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://vyo.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ouw.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ttm.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://bdz.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://kbi.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://afq.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iuq.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://iyz.jinyuanbaomall.cn

[G10] 访问控制
来源：http://afn.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://rge.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://shd.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://lrq.hammf.cn

TS:   public / protected / private
来源：http://kqr.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://ool.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://utj.zhixingplan.top

Ruby: public / protected / private
来源：http://ozl.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://jsg.ydjk.org.cn

[G11] getter / setter
来源：http://nsp.fengsongda.top

Py:   @property 与 @x.setter
来源：http://jxz.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cug.andypj.xyz

JS:   get name() { return this._name; }
来源：http://kcr.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://gvb.sysykeji.top

Java: public String getName() { return name; }
来源：http://ckp.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://gby.cashguo.top

Ruby: attr_accessor :name
来源：http://oqs.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://vwj.nwbrower.top

[G12] 对象转字符串
来源：http://wnj.nanxinkj.top

Py:   def __str__(self): return self.name
来源：http://ikq.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rej.zycfv.cn

JS:   toString() { return this.name; }
来源：http://jia.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://kaa.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://iht.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://esl.52xcode.cn

Ruby: def to_s; @name; end
来源：http://dpi.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://bvo.hysaishi.cn

[G13] 判断对象类型
来源：http://zgj.tarul.cn

Py:   isinstance(u, User)
来源：http://uxi.dashuyun.cn

PHP:  $u instanceof User
来源：http://jwi.daria6918.cn

JS:   u instanceof User
来源：http://yxo.snrcjt.cn

TS:   u instanceof User
来源：http://cgc.jinqigfzy.top

Java: u instanceof User
来源：http://lmw.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://qkk.cucudq.cn

Ruby: u.is_a?(User)
来源：http://sih.xuanzx.com

C#:   u is User
来源：http://sma.ctjpmb.com

[G14] 数据类 / record
来源：http://yif.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kqw.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://psz.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fis.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://aoh.yuxming.cn

Java: record User(String name, int age) {}
来源：http://yrw.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://ekq.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bdg.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://ipv.yuxming.cn

[G15] 枚举
来源：http://mhg.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xdc.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ypj.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wjq.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fnf.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://hsu.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lkb.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://mfp.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://onb.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://uxw.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dut.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://mdc.svipenyu.cn

JS:   Object.entries(obj)
来源：http://glr.guowangkeji.top

TS:   Object.entries(obj)
来源：http://wts.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ifm.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jds.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://nkh.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://cah.zhongyouzk.top

================================================================================
来源：http://xjc.pengpengdd.cyou

H. 异常与错误处理
来源：http://icn.yangfankeji.com

================================================================================
来源：http://bjx.zycfv.cn

[H01] try / catch 基础
来源：http://owv.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mcl.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vtm.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://suq.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yth.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vyy.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hvy.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vln.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://khn.cucudq.cn

[H02] finally / ensure 收尾
来源：http://qtt.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://cmt.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tdr.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eav.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gha.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pot.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://oxt.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yir.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kpb.jlsjyb.cn

[H03] 主动抛出异常
来源：http://avd.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://ocg.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ian.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://tco.zhijiandao.cn

TS:   throw new Error("错误信息");
来源：http://pvn.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://lct.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iwf.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ysb.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://puw.yangfankeji.com

[H04] 自定义异常类型
来源：http://oku.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://ams.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nhm.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://vpr.fzhhl.top

TS:   class MyError extends Error {}
来源：http://zjd.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://nhj.cucudq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://znm.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://xmt.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://ure.wangdashe.top

[H05] 捕获特定类型
来源：http://pae.nanxinkj.top

Py:   except ValueError as e:
来源：http://pfy.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://axi.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://tzx.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://lue.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://gsz.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yfm.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://vjp.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dgn.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://iui.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://gcr.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://cxy.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://ieb.zhoulong.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://kko.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ejl.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rem.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://kax.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://nvj.ydzc1.top

[H07] 断言
来源：http://btx.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://vye.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://wjt.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://jtq.316326.xyz

TS:   console.assert(x > 0);
来源：http://hvo.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://kqj.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hna.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://hxv.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://lku.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://mcj.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://szv.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jpl.sysykeji.top

JS:   e.message;  e.stack
来源：http://rde.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pjz.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fcz.cqqwz.cn

Go:   err.Error()
来源：http://wqb.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://azo.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://yng.9152youxi.cn

[H09] 带错误码的异常
来源：http://cqx.guowangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zjc.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://axl.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fac.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kjb.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qaj.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ifh.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://rbc.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nnu.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://hhm.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://plm.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yed.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pna.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jnp.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://thc.feifeiyinyue.top

Go:   defer f.Close()
来源：http://mts.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qvs.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wdf.nanxuanxn.top

================================================================================
来源：http://xrb.dianchejie.cn

I. 正则表达式
来源：http://cyn.jqgfzy.top

================================================================================
来源：http://lvg.cucudq.cn

[I01] 判断是否匹配
来源：http://tkl.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vvu.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://bic.tanke756.top

JS:   /\d+/.test(s)
来源：http://xoo.hesvh.cn

TS:   /\d+/.test(s)
来源：http://rsn.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wxk.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ytq.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://cjf.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vwn.zhongyouzk.top

[I02] 提取所有匹配
来源：http://hwo.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://esr.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://myz.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bpt.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://cie.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hrn.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fja.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://njf.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aqy.chenlongwang.top

[I03] 提取捕获分组
来源：http://wpk.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://imf.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mxb.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tno.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qro.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://moo.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aim.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bac.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://avb.nanxinkj.top

[I04] 正则替换
来源：http://lrc.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://akb.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lcm.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://hug.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://efm.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://dwy.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://enc.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://agi.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jze.hongshengwenyu.top

[I05] 按正则拆分
来源：http://kvi.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qbo.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bjx.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://eub.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://jly.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://hpu.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://han.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://wvh.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zpc.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hul.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xni.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lli.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mek.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lfs.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ill.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uwh.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wni.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://usj.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://kkp.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tib.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://swz.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jhs.sysykeji.top

TS:   /error/gim
来源：http://gal.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nsf.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jxu.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://fuc.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wwa.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://hex.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gqh.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jpl.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tpd.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mmo.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jab.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bqo.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xba.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nkw.tanke756.top

================================================================================
来源：http://zeo.zhaomingkeji.xyz

J. 日期与时间
来源：http://lom.xuanzx.com

================================================================================
来源：http://bkd.gaohongyu789.top

[J01] 获取当前时间
来源：http://ean.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rwk.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qzt.iojbl.cn

JS:   new Date();  Date.now()
来源：http://oxe.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://nbj.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://iec.snrcjt.cn

Go:   time.Now()
来源：http://yqt.hysaishi.cn

Ruby: Time.now
来源：http://bpo.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uym.yj20258888.top

[J02] 格式化输出
来源：http://omk.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hzy.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bid.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dte.cqqwz.cn

TS:   d.toISOString()
来源：http://ycg.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yvw.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tdy.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lsc.xuanzx.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gdj.gotoacloud.top

[J03] 字符串解析为日期
来源：http://qrz.andypj.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rie.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jvy.316326.xyz

JS:   new Date("2024-01-02")
来源：http://qzz.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://hmq.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://tiz.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sij.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://rnx.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qrx.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://wgn.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://edk.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mlg.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fas.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lzp.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ndk.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yxz.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sjo.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tsr.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://axg.cheryme.top

Py:   now + timedelta(days=7)
来源：http://iyj.xuetiantiany.cn


<!-- 参考信息 -->