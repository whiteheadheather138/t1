代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://sra.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://lyo.hesvh.cn

Py:   super().greet()
来源：http://saw.gotoacloud.top

PHP:  parent::greet();
来源：http://vag.dashuyun.cn

JS:   super.greet();
来源：http://sgv.xuetiantiany.cn

TS:   super.greet();
来源：http://obv.feifeiyinyue.top

Java: super.greet();
来源：http://vfn.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dlf.chenzaomai.com

Ruby: super
来源：http://sxh.ydjk.org.cn

C#:   base.Greet();
来源：http://mwj.tian-w.cn

[G08] 静态方法与属性
来源：http://icz.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fga.sysykeji.top

PHP:  public static function f() {}
来源：http://non.gotoacloud.top

JS:   static f() {}
来源：http://usw.fzhhl.top

TS:   static f(): void {}
来源：http://kfq.ctjpmb.com

Java: static void f() {}
来源：http://plt.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qey.zhijiandao.cn

Ruby: def self.f; end
来源：http://rgd.aibaodan.cn

C#:   public static void F() {}
来源：http://ybf.hnqzz.top

[G09] 接口 / 抽象类
来源：http://xda.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://vjy.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://bdi.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://fpn.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://fze.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://mtf.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://del.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pkh.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://dcn.tanke756.top

[G10] 访问控制
来源：http://dls.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://vxv.daria6918.cn

PHP:  public / protected / private
来源：http://bcj.xuanzx.com

JS:   #private 字段；其余公开
来源：http://wxk.c1oappe.top

TS:   public / protected / private
来源：http://jub.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://hzk.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rta.vqdsnc.cn

Ruby: public / protected / private
来源：http://lce.svipenyu.cn

C#:   public / protected / private / internal
来源：http://gkb.svipenyu.cn

[G11] getter / setter
来源：http://ymp.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://uap.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fwm.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://yql.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://pfg.hcnkem.com

Java: public String getName() { return name; }
来源：http://soq.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hhy.zhengqikj.top

Ruby: attr_accessor :name
来源：http://lgn.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://wed.zhengqikj.top

[G12] 对象转字符串
来源：http://isq.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://afc.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jeh.nwbrower.top

JS:   toString() { return this.name; }
来源：http://jgl.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://dhp.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://wdf.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ypy.xuanzx.com

Ruby: def to_s; @name; end
来源：http://ghy.feifeiyinyue.top

C#:   public override string ToString() => Name;
来源：http://qwr.jyoumei.cn

[G13] 判断对象类型
来源：http://mro.tanke756.top

Py:   isinstance(u, User)
来源：http://suo.vehdjk.com

PHP:  $u instanceof User
来源：http://fmi.fengsongda.top

JS:   u instanceof User
来源：http://osx.hfpthk.cn

TS:   u instanceof User
来源：http://bew.hywenlv.cn

Java: u instanceof User
来源：http://vyx.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nxl.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://mnh.hnxiangtu.top

C#:   u is User
来源：http://sgi.c1oappe.top

[G14] 数据类 / record
来源：http://baz.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wrw.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://nqn.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://olp.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://wju.andypj.xyz

Java: record User(String name, int age) {}
来源：http://giu.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://jup.ybcxt.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aix.cashguo.top

C#:   record User(string Name, int Age);
来源：http://oyr.yfazqb.com

[G15] 枚举
来源：http://zdq.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hbq.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://txm.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zjm.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wuw.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://dxs.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fqt.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://hdy.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ytd.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://dmt.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xiy.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://nxs.jiagoushi.top

JS:   Object.entries(obj)
来源：http://xco.hesvh.cn

TS:   Object.entries(obj)
来源：http://glb.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wfz.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ivq.hammf.cn

Ruby: obj.instance_variables
来源：http://zcl.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://zjo.shzxlz.cn

================================================================================
来源：http://iqz.jqgufenzy.top

H. 异常与错误处理
来源：http://urx.jiagoushi.top

================================================================================
来源：http://nyc.vqdsnc.cn

[H01] try / catch 基础
来源：http://ruq.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kmw.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jcp.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qvx.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sxp.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://snf.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wmc.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ulf.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fqy.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://dpr.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://irl.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dsg.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sra.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fhr.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://kld.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zxr.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://bvc.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://clu.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://zam.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://vnj.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wnv.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://gbh.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://ckw.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xnt.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tvq.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://chh.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://rcy.nanxuanxn.top

[H04] 自定义异常类型
来源：http://jkp.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://ufw.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://afc.aizwys.cn

JS:   class MyError extends Error {}
来源：http://tbo.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://ouy.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://ipr.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gpe.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://agn.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://sbl.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://oaz.ydzc1.top

Py:   except ValueError as e:
来源：http://ugl.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xdc.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://rbg.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://yba.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://jzf.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://deh.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://syz.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://llj.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://qml.52xcode.cn

Py:   value = d.get("k") or default
来源：http://svn.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mpp.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://fzv.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://uri.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bmr.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://rjn.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://rkj.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://jgq.hnqzz.top

[H07] 断言
来源：http://nwy.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://nsa.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://ius.fzhhl.top

JS:   console.assert(x > 0);
来源：http://apz.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://izp.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://sfv.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uos.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://fzt.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://dpg.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://mnb.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://osv.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lop.zhengqikj.top

JS:   e.message;  e.stack
来源：http://ubi.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://nox.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qjb.jiagoushi.top

Go:   err.Error()
来源：http://tlv.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://cpo.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://ijl.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://eub.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qnd.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qgh.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://whq.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dqy.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nbb.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://csw.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://ldc.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rzq.9152youxi.cn

[H10] 资源自动释放
来源：http://fkh.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wsd.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qfu.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rlb.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zva.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lfx.pycfn.com

Go:   defer f.Close()
来源：http://soa.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://add.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nwq.316326.xyz

================================================================================
来源：http://jyz.andypj.xyz

I. 正则表达式
来源：http://nxt.gotoacloud.top

================================================================================
来源：http://cev.xylfe.cn

[I01] 判断是否匹配
来源：http://hjv.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yaa.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://rdm.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://jzh.fzhhl.top

TS:   /\d+/.test(s)
来源：http://yyo.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://srq.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rkw.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://kty.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tpt.birdmap.top

[I02] 提取所有匹配
来源：http://qiw.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://xvq.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dhr.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ama.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://vtr.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cxt.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fsc.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://fiz.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dgb.pycfn.com

[I03] 提取捕获分组
来源：http://pac.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ddp.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://okb.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kmz.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hiz.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://off.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ptw.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://imv.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nmp.gaohongyu789.top

[I04] 正则替换
来源：http://fxr.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lwf.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pdg.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://vub.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://tmm.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oxj.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://utt.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zhq.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yst.hfpthk.cn

[I05] 按正则拆分
来源：http://qfp.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uur.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://reg.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://lmm.ydzc1.top

TS:   s.split(/\s*,\s*/)
来源：http://wpx.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://qxu.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wpm.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://hnt.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xfv.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tat.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gdg.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zma.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ayp.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enh.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hhr.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nhc.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uyz.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qqm.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://slb.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://erp.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uxc.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jvz.sxryk.cn

TS:   /error/gim
来源：http://rar.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://coz.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vir.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://gnu.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pqp.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://anx.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qfs.epnwcf.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cbk.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ekl.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qiy.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://lwv.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gwt.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fag.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pqk.zhongyouzk.top

================================================================================
来源：http://hsk.svipenyu.cn

J. 日期与时间
来源：http://vkd.zhengqikj.top

================================================================================
来源：http://gkl.zhixingplan.top

[J01] 获取当前时间
来源：http://ral.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vtt.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kkd.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://ndq.snrcjt.cn

TS:   new Date();  Date.now()
来源：http://rbj.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://txs.gogol.net.cn

Go:   time.Now()
来源：http://gpy.xuetiantiany.cn

Ruby: Time.now
来源：http://avx.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mhj.sjlbkw.cn

[J02] 格式化输出
来源：http://jvb.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uhr.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dkx.aibaodan.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gzc.bbcook.cn

TS:   d.toISOString()
来源：http://ikg.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qge.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dwq.xingfuxueyuan.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cnl.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wmm.hywenlv.cn

[J03] 字符串解析为日期
来源：http://idp.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yvo.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fyt.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://dex.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://ulf.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lsv.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bgd.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://kon.aizwys.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://djc.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://kke.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bfc.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://czk.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fzg.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ebr.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fsd.hysaishi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wbn.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vzf.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pmb.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://clq.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://cov.havefunace.top


<!-- 参考信息 -->