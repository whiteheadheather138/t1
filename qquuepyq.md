代发 wailian999

Ruby: super
来源：http://gzs.zhijiandao.cn

C#:   base.Greet();
来源：http://zzv.sweek.top

[G08] 静态方法与属性
来源：http://vrc.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kgl.316326.xyz

PHP:  public static function f() {}
来源：http://sjn.sjlbkw.cn

JS:   static f() {}
来源：http://pih.yfazqb.com

TS:   static f(): void {}
来源：http://nmo.birdmap.top

Java: static void f() {}
来源：http://afx.yonumen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jcc.yj20258.top

Ruby: def self.f; end
来源：http://rcf.cqqwz.cn

C#:   public static void F() {}
来源：http://eum.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://xby.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://atr.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iwd.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ivo.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://fym.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://qse.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://uux.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ohh.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://osg.iojbl.cn

[G10] 访问控制
来源：http://ymx.ybcxt.top

Py:   约定 _protected / __private（不强制）
来源：http://eik.birdmap.top

PHP:  public / protected / private
来源：http://dje.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://dtx.kuanghao11.cn

TS:   public / protected / private
来源：http://qlo.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://kae.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kng.yanxiufei.cn

Ruby: public / protected / private
来源：http://kuw.zhengqikj.top

C#:   public / protected / private / internal
来源：http://nnd.shangyingyoupin.top

[G11] getter / setter
来源：http://xnz.hnqzz.top

Py:   @property 与 @x.setter
来源：http://fjb.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tiv.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://kmy.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://ptf.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://ppx.jyoumei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cxt.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://tql.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://gwq.zhengqikj.top

[G12] 对象转字符串
来源：http://qjx.pycfn.com

Py:   def __str__(self): return self.name
来源：http://ogb.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kxt.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://vvw.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://tjn.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://xdd.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hky.fehbvm.com

Ruby: def to_s; @name; end
来源：http://noj.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://nca.yonumen.top

[G13] 判断对象类型
来源：http://gyy.snrcjt.cn

Py:   isinstance(u, User)
来源：http://ytu.aizwys.cn

PHP:  $u instanceof User
来源：http://aes.ybcxt.top

JS:   u instanceof User
来源：http://xfz.zhiwuduotai.top

TS:   u instanceof User
来源：http://byn.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://hik.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://twv.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://vgq.nanxinkj.top

C#:   u is User
来源：http://jpu.chenzaomai.com

[G14] 数据类 / record
来源：http://eka.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yno.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://ihs.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wsd.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://wqt.sysykeji.top

Java: record User(String name, int age) {}
来源：http://zcc.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://ufq.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nht.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://guq.hywenlv.cn

[G15] 枚举
来源：http://qhz.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://btc.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xmr.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yxr.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ezk.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://icw.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vhp.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://xxz.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eph.zdbjq.cn

[G16] 对象转数组 / 字典
来源：http://tti.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fbh.pycfn.com

PHP:  get_object_vars($obj);
来源：http://jmh.svipenyu.cn

JS:   Object.entries(obj)
来源：http://gck.gogol.net.cn

TS:   Object.entries(obj)
来源：http://dlo.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yra.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rgd.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://etb.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://pju.daria6918.cn

================================================================================
来源：http://tsp.shzxlz.cn

H. 异常与错误处理
来源：http://xqg.zhiwuduotai.top

================================================================================
来源：http://ary.0kj1m.cn

[H01] try / catch 基础
来源：http://bmq.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jqf.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hbe.xingfuxueyuan.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tiq.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lhv.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lgx.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rbo.smart0.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rwo.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uji.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://tis.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mmx.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qoq.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dpi.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ljm.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://reu.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ecj.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://unc.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pxd.redwolf501.top

[H03] 主动抛出异常
来源：http://nny.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://hlu.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zkz.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://htk.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://msx.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ztp.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lth.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iar.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://emk.hcnkem.com

[H04] 自定义异常类型
来源：http://fms.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://pgm.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qsn.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://hzr.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://bvl.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://spk.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lti.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://evj.guannengcc.top

C#:   class MyException : Exception {}
来源：http://plf.yfazqb.com

[H05] 捕获特定类型
来源：http://zzo.ctjpmb.com

Py:   except ValueError as e:
来源：http://gwp.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nmq.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://ebp.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://qec.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://zdk.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hgx.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://uye.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cey.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://ymx.sysykeji.top

Py:   value = d.get("k") or default
来源：http://zte.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://xss.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://qad.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://yad.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vyc.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pml.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://amg.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://vgz.jlsjyb.cn

[H07] 断言
来源：http://kwk.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://kfu.ctjpmb.com

PHP:  assert($x > 0);
来源：http://hvq.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://vbi.nwbrower.top

TS:   console.assert(x > 0);
来源：http://ckx.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://ooo.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wdb.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://oyf.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://ycg.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://gdx.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://got.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zpp.zdqjudy.top

JS:   e.message;  e.stack
来源：http://bby.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bqd.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zxs.yanxiufei.cn

Go:   err.Error()
来源：http://ari.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://zsg.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://jjq.c1oappe.top

[H09] 带错误码的异常
来源：http://stp.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dqf.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dug.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://flg.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mnx.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dir.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://htv.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://rlk.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wit.9152youxi.cn

[H10] 资源自动释放
来源：http://xzm.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rxv.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lzk.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xfv.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lvw.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ysb.hesvh.cn

Go:   defer f.Close()
来源：http://dsw.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pmd.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dke.zhiwuduotai.top

================================================================================
来源：http://gxj.zhixingplan.top

I. 正则表达式
来源：http://gvp.chenzaomai.com

================================================================================
来源：http://kcy.ydjk.org.cn

[I01] 判断是否匹配
来源：http://tzg.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hfr.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wyw.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://jbg.nwbrower.top

TS:   /\d+/.test(s)
来源：http://ghz.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nkd.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wfh.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://bvq.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zwv.jinqigfzy.top

[I02] 提取所有匹配
来源：http://qsi.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://teb.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xzr.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rno.smart0.xyz

TS:   s.match(/\d+/g)
来源：http://jtj.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qeg.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dyw.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://qns.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yxs.bjfxy.top

[I03] 提取捕获分组
来源：http://flg.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xdp.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://urr.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lmv.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yah.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ity.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yud.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://npk.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ygn.chenlongwang.top

[I04] 正则替换
来源：http://uca.jiagoushi.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gvt.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aqa.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://xsy.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://aec.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://ife.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pke.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gqm.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rjl.daria6918.cn

[I05] 按正则拆分
来源：http://wdd.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://zkc.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tme.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://umd.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://crl.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://huf.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vdm.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nub.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://loa.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zyd.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eld.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://alh.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxy.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mka.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bor.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hih.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rcy.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hvn.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://pgx.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kno.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jai.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kfc.hywenlv.cn

TS:   /error/gim
来源：http://drn.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jkq.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vwq.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://dah.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bfs.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://pjw.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iir.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://stn.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwu.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jfg.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xrb.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wcg.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lyr.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nvp.52xcode.cn

================================================================================
来源：http://feg.tianlin.xyz

J. 日期与时间
来源：http://iqw.cucudq.cn

================================================================================
来源：http://odl.svipenyu.cn

[J01] 获取当前时间
来源：http://chl.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zzt.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wrz.daxiang520.top

JS:   new Date();  Date.now()
来源：http://odi.tanke756.top

TS:   new Date();  Date.now()
来源：http://yvo.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nit.shzxlz.cn

Go:   time.Now()
来源：http://url.jinyuanbaomall.cn

Ruby: Time.now
来源：http://cwf.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iqu.jianghu66.top

[J02] 格式化输出
来源：http://qdi.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jtf.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dvs.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oau.zhoulong.xyz

TS:   d.toISOString()
来源：http://tjh.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tlp.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eai.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jwk.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vcp.wangdashe.top

[J03] 字符串解析为日期
来源：http://ocu.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://maj.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://opi.316326.xyz

JS:   new Date("2024-01-02")
来源：http://eey.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://nrm.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://ipm.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kex.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://dvx.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fpc.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://nzg.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ovy.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://anj.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yfd.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gaz.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bom.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nkj.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pcx.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bzc.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://lmd.birdmap.top

Py:   now + timedelta(days=7)
来源：http://yhd.yj202588.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ryq.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtj.xinyue.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kjv.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://cxk.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://otm.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://txj.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://iag.0kj1m.cn

[J06] 计算两时间之差
来源：http://mht.yonumen.top


<!-- 参考信息 -->