代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://fif.cdnleiting.top

[G07] 调用父类方法
来源：http://vvt.yvedp.cn

Py:   super().greet()
来源：http://kpc.jqgfzy.top

PHP:  parent::greet();
来源：http://okh.yueranfly.top

JS:   super.greet();
来源：http://dip.ppjwa.cn

TS:   super.greet();
来源：http://wqn.jinghuilouyu.cn

Java: super.greet();
来源：http://nuo.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qrn.yfazqb.com

Ruby: super
来源：http://dnr.yangfankeji.com

C#:   base.Greet();
来源：http://uxq.chenzaomai.com

[G08] 静态方法与属性
来源：http://dro.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dra.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://fsk.xuanzx.com

JS:   static f() {}
来源：http://ozz.cheryme.top

TS:   static f(): void {}
来源：http://fid.xinyue.icu

Java: static void f() {}
来源：http://yrk.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://epf.aizwys.cn

Ruby: def self.f; end
来源：http://fyl.zhengqikj.top

C#:   public static void F() {}
来源：http://dcc.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://enx.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://amr.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mkl.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vsc.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://oha.tarul.cn

Java: interface Shape { double area(); }
来源：http://djt.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://zrl.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mjc.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://ont.vqdsnc.cn

[G10] 访问控制
来源：http://gih.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://rsz.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://arq.tarul.cn

JS:   #private 字段；其余公开
来源：http://cem.zhiwuduotai.top

TS:   public / protected / private
来源：http://zlr.yj202588.top

Java: public / protected / private / 默认包级
来源：http://pyt.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rrs.jyoumei.cn

Ruby: public / protected / private
来源：http://acd.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://emp.52xcode.cn

[G11] getter / setter
来源：http://qpo.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://rpy.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zav.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://ypv.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://qkh.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://eon.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://dqe.zhixingplan.top

Ruby: attr_accessor :name
来源：http://xag.yvedp.cn

C#:   public string Name { get; set; }
来源：http://kdk.gotoacloud.top

[G12] 对象转字符串
来源：http://jms.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://hup.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://prr.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://sfe.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://zwd.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://jbi.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://gzw.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://vcz.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://vqn.hcnkem.com

[G13] 判断对象类型
来源：http://lfj.bbcook.cn

Py:   isinstance(u, User)
来源：http://ybn.hfpthk.cn

PHP:  $u instanceof User
来源：http://dbt.epnwcf.com

JS:   u instanceof User
来源：http://nlu.cashguo.top

TS:   u instanceof User
来源：http://huf.yj202588.top

Java: u instanceof User
来源：http://iti.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nvi.meibo888.top

Ruby: u.is_a?(User)
来源：http://fwg.fanxiaobao.xyz

C#:   u is User
来源：http://qhc.fengsongda.top

[G14] 数据类 / record
来源：http://eka.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ddh.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://zal.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://huh.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://adr.hammf.cn

Java: record User(String name, int age) {}
来源：http://yyi.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://dhi.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ser.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://mgb.jinqigufen.top

[G15] 枚举
来源：http://oky.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pjg.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cbi.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nvj.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://syo.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://zwt.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://flq.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://drj.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://efy.cucudq.cn

[G16] 对象转数组 / 字典
来源：http://iym.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://abd.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://zzd.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://cek.daxiang520.top

TS:   Object.entries(obj)
来源：http://kkx.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nxu.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nuz.xinyue.icu

Ruby: obj.instance_variables
来源：http://pju.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://hej.dianchejie.cn

================================================================================
来源：http://joe.52xcode.cn

H. 异常与错误处理
来源：http://jrp.zhaomingkeji.xyz

================================================================================
来源：http://lrz.tarul.cn

[H01] try / catch 基础
来源：http://zit.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hhw.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bmr.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vbj.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://geb.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dph.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kvx.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://emd.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gvt.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://iaq.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://jji.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kjo.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jut.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xft.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://rya.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://tfd.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ycy.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ras.aizwys.cn

[H03] 主动抛出异常
来源：http://rti.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://fik.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kpf.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://ndg.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://hdo.yongpay.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zvx.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://csa.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://nig.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://cjn.c1oappe.top

[H04] 自定义异常类型
来源：http://gsq.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://xuq.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://jyw.xuanzx.com

JS:   class MyError extends Error {}
来源：http://zak.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://fjt.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://drt.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cvg.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://sxp.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://yzq.aizwys.cn

[H05] 捕获特定类型
来源：http://pia.zhengqikj.top

Py:   except ValueError as e:
来源：http://zjp.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nou.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://cnr.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://grz.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://cvx.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rfc.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://gzz.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xur.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://tlu.yonumen.top

Py:   value = d.get("k") or default
来源：http://got.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://hjx.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://jyi.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://nuu.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ivw.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xog.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://fzh.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://bvt.jiagoushi.top

[H07] 断言
来源：http://pzx.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://pph.ehwqpu.com

PHP:  assert($x > 0);
来源：http://erc.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://aan.yj20258.top

TS:   console.assert(x > 0);
来源：http://xfo.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://nvh.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uyc.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rxb.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://ard.sweek.top

[H08] 获取错误信息与堆栈
来源：http://rzr.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://jtm.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ibl.hfpthk.cn

JS:   e.message;  e.stack
来源：http://ktz.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bgy.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://qlt.zhaomingkeji.xyz

Go:   err.Error()
来源：http://fiq.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://ign.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://cpp.zdbjq.cn

[H09] 带错误码的异常
来源：http://mua.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qfw.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://gjl.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pdo.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wbh.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gku.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pqz.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://bdj.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yin.bbcook.cn

[H10] 资源自动释放
来源：http://khg.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://onj.wangdashe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hcx.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gdw.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xgl.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wbw.yongpay.top

Go:   defer f.Close()
来源：http://wbz.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aht.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hmt.dianchejie.cn

================================================================================
来源：http://wyk.uphjek.com

I. 正则表达式
来源：http://ysr.yuxming.cn

================================================================================
来源：http://eru.yuanzhike.top

[I01] 判断是否匹配
来源：http://jjq.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://stw.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ukg.birdmap.top

JS:   /\d+/.test(s)
来源：http://ikp.yj202588.top

TS:   /\d+/.test(s)
来源：http://gsp.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vgt.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://suh.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://lvs.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uhw.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://tzv.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://ctm.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oss.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nyy.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://anp.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xbf.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tny.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://tfo.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dmf.xinyue.icu

[I03] 提取捕获分组
来源：http://ayg.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://elk.ybcxt.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qfi.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mww.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lru.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ulf.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jjh.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pnn.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fqn.yj20258.top

[I04] 正则替换
来源：http://mtn.9152youxi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hby.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yip.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vea.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://krp.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://yaz.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vys.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://imn.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gwo.chenlongwang.top

[I05] 按正则拆分
来源：http://gwy.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tkd.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eay.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://kiu.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://tbz.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://dtj.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hci.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://bpm.zhixingplan.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ieu.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zhn.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pcj.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tmz.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://srh.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eri.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wcm.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yuc.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tob.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kij.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://iqj.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://imt.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pwa.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dqb.sxryk.cn

TS:   /error/gim
来源：http://qxi.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uij.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jta.uphjek.com

Ruby: s.scan(/error/i)
来源：http://uck.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rtc.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://nhe.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jzp.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uwa.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lyp.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nmj.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lit.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dql.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rur.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mzf.sufxvd.cn

================================================================================
来源：http://tgc.ydzc1.top

J. 日期与时间
来源：http://xzd.daria6918.cn

================================================================================
来源：http://vln.zhixingplan.top

[J01] 获取当前时间
来源：http://hnm.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ikw.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vyt.hammf.cn

JS:   new Date();  Date.now()
来源：http://gop.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://qfw.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yfj.hesvh.cn

Go:   time.Now()
来源：http://cts.xylfe.cn

Ruby: Time.now
来源：http://lkf.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zvx.xziqi.cn

[J02] 格式化输出
来源：http://mfv.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wyz.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wqs.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fdf.hywenlv.cn

TS:   d.toISOString()
来源：http://dso.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rhs.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zzc.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://llc.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cgq.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://gdu.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bdb.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ahj.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://esq.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://mhb.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://dmi.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qxz.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://dct.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ewj.zycfv.cn

[J04] 时间戳与日期互转
来源：http://xnx.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lvs.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pta.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nhp.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fvz.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mdr.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://opx.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lgt.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fmk.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://fju.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://tby.shanyushiyangkeji.top


<!-- 参考信息 -->