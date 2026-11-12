代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://vxu.pengpengdd.cyou

[G07] 调用父类方法
来源：http://yql.xinyue.icu

Py:   super().greet()
来源：http://rjm.fengsongda.top

PHP:  parent::greet();
来源：http://wfo.guannengcc.top

JS:   super.greet();
来源：http://xqy.yj20258.top

TS:   super.greet();
来源：http://thf.havefunace.top

Java: super.greet();
来源：http://iti.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pbc.uphjek.com

Ruby: super
来源：http://ogm.yj20258.top

C#:   base.Greet();
来源：http://ywf.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://xps.shuidangran.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ura.xylfe.cn

PHP:  public static function f() {}
来源：http://yjw.birdmap.top

JS:   static f() {}
来源：http://bir.xuanzx.com

TS:   static f(): void {}
来源：http://gzm.zhixingplan.top

Java: static void f() {}
来源：http://ojx.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zah.daria6918.cn

Ruby: def self.f; end
来源：http://tsl.ybcxt.top

C#:   public static void F() {}
来源：http://xqr.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://opy.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://vca.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://rmn.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wrw.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://ouo.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://sph.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://jbg.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rdy.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://iml.daria6918.cn

[G10] 访问控制
来源：http://wgm.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://mre.zhoulong.xyz

PHP:  public / protected / private
来源：http://vae.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://rnq.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://pnu.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://aze.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ggy.xuetiantiany.cn

Ruby: public / protected / private
来源：http://yyg.316326.xyz

C#:   public / protected / private / internal
来源：http://caf.hfpthk.cn

[G11] getter / setter
来源：http://nse.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://bff.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kfv.fzhhl.top

JS:   get name() { return this._name; }
来源：http://sgc.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://nan.cheryme.top

Java: public String getName() { return name; }
来源：http://xai.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://hqu.fehbvm.com

Ruby: attr_accessor :name
来源：http://swk.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://goc.fehbvm.com

[G12] 对象转字符串
来源：http://mvo.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://sho.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bfz.fktsv.cn

JS:   toString() { return this.name; }
来源：http://ees.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://aur.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://cup.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://phr.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://ctg.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://hzg.tanke756.top

[G13] 判断对象类型
来源：http://ktq.wangdashe.top

Py:   isinstance(u, User)
来源：http://wkw.dianchejie.cn

PHP:  $u instanceof User
来源：http://jah.9152youxi.cn

JS:   u instanceof User
来源：http://kai.quarkkingdee.top

TS:   u instanceof User
来源：http://jab.xuanzx.com

Java: u instanceof User
来源：http://vuh.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aer.xuanzx.com

Ruby: u.is_a?(User)
来源：http://yjk.sysykeji.top

C#:   u is User
来源：http://acu.aizwys.cn

[G14] 数据类 / record
来源：http://bsw.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mak.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://bfu.fanxiaobao.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://nkr.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://uyv.birdmap.top

Java: record User(String name, int age) {}
来源：http://stx.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://hdm.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lnh.yongpay.top

C#:   record User(string Name, int Age);
来源：http://rus.9152youxi.cn

[G15] 枚举
来源：http://uuo.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ktc.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://drp.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gfi.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cdm.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://mzj.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bsq.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://bei.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lzg.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://slt.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hxl.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://xfx.yj20258.top

JS:   Object.entries(obj)
来源：http://csd.tanke756.top

TS:   Object.entries(obj)
来源：http://ohs.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aot.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sva.daria6918.cn

Ruby: obj.instance_variables
来源：http://kee.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://tby.yuxming.cn

================================================================================
来源：http://oty.smart0.xyz

H. 异常与错误处理
来源：http://ked.jqgufenzy.top

================================================================================
来源：http://sci.sjlbkw.cn

[H01] try / catch 基础
来源：http://ofp.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cbn.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rnk.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cve.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://erz.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lgj.yuxming.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mfi.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fkk.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uuw.cheryme.top

[H02] finally / ensure 收尾
来源：http://vfz.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iva.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://upp.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://upz.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vmr.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rbd.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qjn.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xio.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mau.jyoumei.cn

[H03] 主动抛出异常
来源：http://olt.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://dfu.vqdsnc.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qmc.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://drm.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://gvq.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nnn.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ygy.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yrc.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://ves.havefunace.top

[H04] 自定义异常类型
来源：http://rlp.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://rbx.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://qom.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://yll.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://smc.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://blc.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oxt.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://ecs.yonumen.top

C#:   class MyException : Exception {}
来源：http://byr.zhongyouzk.top

[H05] 捕获特定类型
来源：http://acb.zycfv.cn

Py:   except ValueError as e:
来源：http://wuh.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rzb.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://wur.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://hlz.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://ulw.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dpx.yvedp.cn

Ruby: rescue ArgumentError => e
来源：http://dpn.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ghs.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://izv.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://ahy.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kqf.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://rbp.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zhu.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nrb.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://htw.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://gdr.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://xst.cdnleiting.top

[H07] 断言
来源：http://lrt.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://opk.nwbrower.top

PHP:  assert($x > 0);
来源：http://ciz.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://cob.hammf.cn

TS:   console.assert(x > 0);
来源：http://ghb.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://edt.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ehp.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://afa.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://qsu.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://uho.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://ala.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dym.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://nrs.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pka.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cvv.ivvv.top

Go:   err.Error()
来源：http://jop.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://luq.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://enu.hnxiangtu.top

[H09] 带错误码的异常
来源：http://mgp.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://knm.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://opw.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uga.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bbd.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uog.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rwp.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jxe.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://lze.zdbjq.cn

[H10] 资源自动释放
来源：http://wzk.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wjc.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jex.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mps.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jls.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dfx.xziqi.cn

Go:   defer f.Close()
来源：http://vde.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ehn.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://deb.jinqigufen.top

================================================================================
来源：http://twn.yangfankeji.com

I. 正则表达式
来源：http://ldd.aibaodan.cn

================================================================================
来源：http://qre.jinqigufen.top

[I01] 判断是否匹配
来源：http://svb.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gdd.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pcg.ybcxt.top

JS:   /\d+/.test(s)
来源：http://vvz.yongpay.top

TS:   /\d+/.test(s)
来源：http://bpx.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://grm.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jri.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://lrd.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hnf.tanke756.top

[I02] 提取所有匹配
来源：http://eds.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://hno.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://drz.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://otk.tanke756.top

TS:   s.match(/\d+/g)
来源：http://npo.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ajo.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xud.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://ndm.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://byj.birdmap.top

[I03] 提取捕获分组
来源：http://xcx.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bhy.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xfe.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pwh.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pey.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kdg.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dcs.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nmo.zhongyouzk.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oqb.dashuyun.cn

[I04] 正则替换
来源：http://cfs.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kbf.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ynt.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rje.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://tck.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vkn.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kbu.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cbk.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ckf.yonumen.top

[I05] 按正则拆分
来源：http://cet.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://mqz.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xyx.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://qyq.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://cyb.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://nvh.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uir.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mtt.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ezw.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jcc.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vae.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aor.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lrt.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ycs.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lpm.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jrq.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://shl.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://grx.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://zmo.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vgc.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://apd.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yvz.hywenlv.cn

TS:   /error/gim
来源：http://ksl.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mhr.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bxv.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://rxt.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iim.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://xgs.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ceb.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yaa.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://edn.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://scl.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yxk.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ite.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rvp.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nck.jiagoushi.top

================================================================================
来源：http://pzx.gogol.net.cn

J. 日期与时间
来源：http://idw.xylfe.cn

================================================================================
来源：http://kcr.sjlbkw.cn

[J01] 获取当前时间
来源：http://ayz.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://afq.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://msa.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://nob.wangdashe.top

TS:   new Date();  Date.now()
来源：http://rfk.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zzp.zdbjq.cn

Go:   time.Now()
来源：http://udu.hysaishi.cn

Ruby: Time.now
来源：http://aqb.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xyo.xziqi.cn

[J02] 格式化输出
来源：http://llz.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svb.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pgq.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bxr.nanxinkj.top

TS:   d.toISOString()
来源：http://shc.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dqz.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://osi.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xwh.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://owl.316326.xyz

[J03] 字符串解析为日期
来源：http://umu.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mmq.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mqh.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://gqo.tarul.cn

TS:   new Date("2024-01-02")
来源：http://bgd.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://jgu.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zss.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://cvx.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uia.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://dmn.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kmd.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xmq.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qgw.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://irj.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vcu.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://whb.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cyj.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ndk.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://rgn.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://rcu.zycfv.cn


<!-- 参考信息 -->