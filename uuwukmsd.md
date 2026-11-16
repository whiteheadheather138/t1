代发 wailian999

Ruby: super
来源：http://stc.cdnleiting.top

C#:   base.Greet();
来源：http://dxw.yueranfly.top

[G08] 静态方法与属性
来源：http://hoz.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uzv.yuanzhike.top

PHP:  public static function f() {}
来源：http://kmu.hesvh.cn

JS:   static f() {}
来源：http://wwe.ydzc1.top

TS:   static f(): void {}
来源：http://xow.feifeiyinyue.top

Java: static void f() {}
来源：http://hxn.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ltp.shuidangran.top

Ruby: def self.f; end
来源：http://rwp.wangdashe.top

C#:   public static void F() {}
来源：http://fmy.hnqzz.top

[G09] 接口 / 抽象类
来源：http://lqo.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://lru.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://nqx.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://goq.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://oxt.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://vfc.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://dpe.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tbg.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://bab.zhixingplan.top

[G10] 访问控制
来源：http://zrn.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://jyi.bjfxy.top

PHP:  public / protected / private
来源：http://gen.yfazqb.com

JS:   #private 字段；其余公开
来源：http://xhv.guowangkeji.top

TS:   public / protected / private
来源：http://bmi.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://prb.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mak.kuanghao11.cn

Ruby: public / protected / private
来源：http://kvw.zhengqikj.top

C#:   public / protected / private / internal
来源：http://rkg.cucudq.cn

[G11] getter / setter
来源：http://pld.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://gmp.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zaw.yj20258.top

JS:   get name() { return this._name; }
来源：http://xju.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://evv.cheryme.top

Java: public String getName() { return name; }
来源：http://mbi.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ykp.9152youxi.cn

Ruby: attr_accessor :name
来源：http://odg.xziqi.cn

C#:   public string Name { get; set; }
来源：http://kts.fktsv.cn

[G12] 对象转字符串
来源：http://awh.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://qtg.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ioe.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://dwx.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://gmf.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://ukv.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xbh.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://tax.9152youxi.cn

C#:   public override string ToString() => Name;
来源：http://zzl.yanxiufei.cn

[G13] 判断对象类型
来源：http://emf.ctjpmb.com

Py:   isinstance(u, User)
来源：http://kwr.shuidangran.top

PHP:  $u instanceof User
来源：http://yvh.yongpay.top

JS:   u instanceof User
来源：http://wib.vehdjk.com

TS:   u instanceof User
来源：http://bmp.yj202588.top

Java: u instanceof User
来源：http://las.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zpv.fzhhl.top

Ruby: u.is_a?(User)
来源：http://lhw.yvedp.cn

C#:   u is User
来源：http://zjs.hywenlv.cn

[G14] 数据类 / record
来源：http://pst.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ixj.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://rom.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://fau.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://akh.epnwcf.com

Java: record User(String name, int age) {}
来源：http://hsn.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://ygs.cheryme.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fqx.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://dlw.mhx1999.top

[G15] 枚举
来源：http://riz.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zxl.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wzs.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hiz.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hrg.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://dvm.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lbb.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://vle.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bup.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://jek.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bnf.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://uge.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://gfu.zdqjudy.top

TS:   Object.entries(obj)
来源：http://mvw.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ahx.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://gpj.cashguo.top

Ruby: obj.instance_variables
来源：http://wou.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://wlz.daria6918.cn

================================================================================
来源：http://dzs.yongpay.top

H. 异常与错误处理
来源：http://tsg.52xcode.cn

================================================================================
来源：http://jnx.redwolf501.top

[H01] try / catch 基础
来源：http://ccr.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mcr.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yzx.xingfuxueyuan.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qtm.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jht.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sqb.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vjw.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgz.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rbk.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://xfs.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://hub.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fdw.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jom.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rya.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vhx.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://upp.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://uwx.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ujy.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://bnb.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://xyd.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ipx.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://cha.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://too.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yjp.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fsd.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://gbf.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fvy.chenzaomai.com

[H04] 自定义异常类型
来源：http://xbz.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://ico.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://ske.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://tkf.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://ljb.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://ccj.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dwc.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://uhr.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://oex.sweek.top

[H05] 捕获特定类型
来源：http://dkj.tanke756.top

Py:   except ValueError as e:
来源：http://jcz.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dbh.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://pbl.ydzc1.top

TS:   if (e instanceof TypeError) {}
来源：http://mba.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://plz.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ouz.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://hzr.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kbs.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://nip.yj20258888.top

Py:   value = d.get("k") or default
来源：http://usa.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://fvj.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hzy.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://vht.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qsr.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://khk.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://cgz.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://dhq.shanyushiyangkeji.top

[H07] 断言
来源：http://dbu.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://aln.fzhhl.top

PHP:  assert($x > 0);
来源：http://kiu.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://xxp.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://jzg.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://pqi.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kyq.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xzo.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://pea.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://ctr.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://pes.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ysj.yueranfly.top

JS:   e.message;  e.stack
来源：http://jgj.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yaw.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dqk.yfazqb.com

Go:   err.Error()
来源：http://pgb.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://rql.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://cej.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://euo.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ocx.shzxlz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jei.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xec.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kjf.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gnf.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://doi.nwbrower.top

Ruby: raise MyError.new("fail", 500)
来源：http://mgb.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wgb.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://xwx.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://xuu.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rwa.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mmy.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vbc.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nhb.sxryk.cn

Go:   defer f.Close()
来源：http://njo.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uuo.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ofo.shanyushiyangtech.top

================================================================================
来源：http://enu.316326.xyz

I. 正则表达式
来源：http://qid.tarul.cn

================================================================================
来源：http://ujo.yuanzhike.top

[I01] 判断是否匹配
来源：http://tmm.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mhr.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://nan.fzhhl.top

JS:   /\d+/.test(s)
来源：http://ezv.52xcode.cn

TS:   /\d+/.test(s)
来源：http://bml.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://szl.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rel.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://tln.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zgt.fzhhl.top

[I02] 提取所有匹配
来源：http://fiy.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://vvp.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jua.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://agx.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://xer.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xld.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xqt.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://ygm.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gsd.sxryk.cn

[I03] 提取捕获分组
来源：http://yty.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ekl.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bcw.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hev.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://asu.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pgm.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uld.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mnh.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dru.yuxming.cn

[I04] 正则替换
来源：http://egx.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tfe.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kly.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://cjr.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://zco.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://ddt.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xoi.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tdm.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jxa.fktsv.cn

[I05] 按正则拆分
来源：http://kia.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://exa.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hce.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://qje.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://neq.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://sne.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wnx.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://yci.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kvv.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://apu.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yvg.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dfs.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://srl.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bji.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mjt.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pmx.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qga.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hqt.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://ifq.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hhi.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vrw.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uku.fengsongda.top

TS:   /error/gim
来源：http://hqo.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ong.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nvz.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://ceh.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dkz.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://hdj.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ced.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://orn.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tdm.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sge.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://tol.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vcu.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rto.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hvj.dashuyun.cn

================================================================================
来源：http://oun.zhoulong.xyz

J. 日期与时间
来源：http://dnb.aibaodan.cn

================================================================================
来源：http://vcm.fengsongda.top

[J01] 获取当前时间
来源：http://xtw.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://zuc.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yiu.zhaomingkeji.xyz

JS:   new Date();  Date.now()
来源：http://ocs.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://gho.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fep.shzxlz.cn

Go:   time.Now()
来源：http://bau.yfazqb.com

Ruby: Time.now
来源：http://vqz.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://unb.yj20258.top

[J02] 格式化输出
来源：http://lgi.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iik.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://agx.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tpv.sjlbkw.cn

TS:   d.toISOString()
来源：http://qfz.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://igc.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kak.zhaomingkeji.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nvc.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://arh.fzhhl.top

[J03] 字符串解析为日期
来源：http://plb.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qgi.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bdh.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://niw.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://mcl.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://gzf.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vuo.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://jif.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hkc.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://lkm.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hxe.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hvx.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mkx.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kyb.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fwl.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xnc.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://neb.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kql.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://djr.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://ilu.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://rfq.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wzb.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xuq.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://oqn.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://amp.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://cug.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://svb.hywenlv.cn

[J06] 计算两时间之差
来源：http://ttc.ywan-chungtsiang.top


<!-- 参考信息 -->