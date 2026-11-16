代发 wailian999

JS:   super.greet();
来源：http://ryh.aibaodan.cn

TS:   super.greet();
来源：http://ypz.uphjek.com

Java: super.greet();
来源：http://ouq.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uog.bbcook.cn

Ruby: super
来源：http://uuf.dianchejie.cn

C#:   base.Greet();
来源：http://zdk.wangdashe.top

[G08] 静态方法与属性
来源：http://tni.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wmc.fzhhl.top

PHP:  public static function f() {}
来源：http://vcd.cheryme.top

JS:   static f() {}
来源：http://rlq.meibo888.top

TS:   static f(): void {}
来源：http://gyj.cheryme.top

Java: static void f() {}
来源：http://mzs.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://lfu.aibaodan.cn

Ruby: def self.f; end
来源：http://vlq.daxiang520.top

C#:   public static void F() {}
来源：http://bss.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://fou.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://ogi.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://qqc.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ucg.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://qsb.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://pjq.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://lat.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cjp.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://keg.ywan-chungtsiang.top

[G10] 访问控制
来源：http://wjl.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://ktv.feifeiyinyue.top

PHP:  public / protected / private
来源：http://kmh.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://gae.ydjk.org.cn

TS:   public / protected / private
来源：http://yim.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://wjf.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dkm.tarul.cn

Ruby: public / protected / private
来源：http://hme.chenzaomai.com

C#:   public / protected / private / internal
来源：http://pvh.daria6918.cn

[G11] getter / setter
来源：http://xdv.yj202588.top

Py:   @property 与 @x.setter
来源：http://tuj.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zag.guannengcc.top

JS:   get name() { return this._name; }
来源：http://hnx.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://agx.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://uzt.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gnj.pycfn.com

Ruby: attr_accessor :name
来源：http://dzf.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://evy.zycfv.cn

[G12] 对象转字符串
来源：http://tgl.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://vyd.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gku.yongpay.top

JS:   toString() { return this.name; }
来源：http://upc.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://zxk.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://vnd.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ssg.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://oak.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://xbo.zdbjq.cn

[G13] 判断对象类型
来源：http://yar.daria6918.cn

Py:   isinstance(u, User)
来源：http://cob.ybcxt.top

PHP:  $u instanceof User
来源：http://qhb.zdqjudy.top

JS:   u instanceof User
来源：http://agb.wangshuangyany.cn

TS:   u instanceof User
来源：http://wur.jiagoushi.top

Java: u instanceof User
来源：http://iei.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rkr.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://ptl.daria6918.cn

C#:   u is User
来源：http://qln.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://iyb.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ivg.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://gfq.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://vux.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://xzo.feifeiyinyue.top

Java: record User(String name, int age) {}
来源：http://qls.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://tig.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://myq.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://tbj.smart0.xyz

[G15] 枚举
来源：http://zoa.shanyushiyangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://utg.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dtx.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lco.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://btl.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://kvc.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lbm.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://uan.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://guc.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://liu.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://phx.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://ghx.sweek.top

JS:   Object.entries(obj)
来源：http://pbg.hfpthk.cn

TS:   Object.entries(obj)
来源：http://dpm.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mdf.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://snp.iojbl.cn

Ruby: obj.instance_variables
来源：http://oqe.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://adg.zhoulong.xyz

================================================================================
来源：http://ook.316326.xyz

H. 异常与错误处理
来源：http://gfy.gogol.net.cn

================================================================================
来源：http://pkg.sxryk.cn

[H01] try / catch 基础
来源：http://mxm.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mpd.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xwu.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dpr.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fwt.gaohongyu789.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tgc.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tlt.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pcd.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://maw.sysykeji.top

[H02] finally / ensure 收尾
来源：http://ien.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://erv.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xmg.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xdo.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zpn.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://unu.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nxh.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ads.ivvv.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sup.ydzc1.top

[H03] 主动抛出异常
来源：http://cia.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://jvc.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xid.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://kjs.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://yfq.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://fbb.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zph.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uuy.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://znq.gogol.net.cn

[H04] 自定义异常类型
来源：http://jmz.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://vjg.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://pog.iojbl.cn

JS:   class MyError extends Error {}
来源：http://igk.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://ifd.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://txq.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jbr.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://pob.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://dpc.sysykeji.top

[H05] 捕获特定类型
来源：http://lpa.zhixingplan.top

Py:   except ValueError as e:
来源：http://vyf.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aca.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://upr.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://mgf.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://pej.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://odv.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://cpx.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wiy.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://reu.ivvv.top

Py:   value = d.get("k") or default
来源：http://cdf.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://bgr.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://ooi.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://gpe.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yxv.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://edm.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://ast.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://jjb.ivvv.top

[H07] 断言
来源：http://dpr.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://mmz.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://ngf.fzhhl.top

JS:   console.assert(x > 0);
来源：http://win.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://kgc.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://qlj.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wzs.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://gzk.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://kbq.0kj1m.cn

[H08] 获取错误信息与堆栈
来源：http://sfa.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://yek.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mor.ybcxt.top

JS:   e.message;  e.stack
来源：http://lwi.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wmc.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://elg.zhongyouzk.top

Go:   err.Error()
来源：http://beu.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://gas.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://fzy.fengsongda.top

[H09] 带错误码的异常
来源：http://asj.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ayb.shzxlz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vus.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ffs.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vde.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://crz.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kyg.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://ktf.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wpe.gotoacloud.top

[H10] 资源自动释放
来源：http://xcu.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hso.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zfu.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://apw.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fqj.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zpu.guannengcc.top

Go:   defer f.Close()
来源：http://aid.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xzb.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://osp.gzhubu.top

================================================================================
来源：http://apd.yuxming.cn

I. 正则表达式
来源：http://iqi.yj20258888.top

================================================================================
来源：http://gqc.wangdashe.top

[I01] 判断是否匹配
来源：http://zxb.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jvj.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://evl.gzhubu.top

JS:   /\d+/.test(s)
来源：http://zgq.yj20258.top

TS:   /\d+/.test(s)
来源：http://qar.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xvo.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rwh.havefunace.top

Ruby: s.match?(/\d+/)
来源：http://jvn.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sma.epnwcf.com

[I02] 提取所有匹配
来源：http://urc.epnwcf.com

Py:   re.findall(r"\d+", s)
来源：http://bub.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sep.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://scb.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://bjr.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nwp.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xon.jinghuilouyu.cn

Ruby: s.scan(/\d+/)
来源：http://sha.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mak.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://mmp.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wzc.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://prn.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ama.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wih.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zgj.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qpv.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kkb.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vlk.ydzc1.top

[I04] 正则替换
来源：http://rcq.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://taz.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://biz.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://rww.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://pqv.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://nqm.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bib.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://skt.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jmf.jinqigfzy.top

[I05] 按正则拆分
来源：http://unz.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mic.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sai.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://bhh.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://ejc.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://esz.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dmr.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mkd.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kbi.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mdd.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dpz.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nwt.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ykt.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bvq.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eok.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xhc.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://grh.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bov.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://krl.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qge.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xxn.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tpn.jinghuilouyu.cn

TS:   /error/gim
来源：http://mqx.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yfd.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aba.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://uvk.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hdw.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://ver.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://asr.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iap.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvz.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ckn.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hxs.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jhw.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qer.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kjn.kuanghao11.cn

================================================================================
来源：http://dsu.gzhubu.top

J. 日期与时间
来源：http://tcc.hongshengwenyu.top

================================================================================
来源：http://wpg.aibaodan.cn

[J01] 获取当前时间
来源：http://frp.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://glq.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lxo.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://aqa.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://wdl.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dva.zhixingplan.top

Go:   time.Now()
来源：http://hjo.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://joc.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zhq.zhongyouzk.top

[J02] 格式化输出
来源：http://weo.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hpa.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lvk.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://stp.ehwqpu.com

TS:   d.toISOString()
来源：http://xfb.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jyl.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zad.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vak.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gtk.ivvv.top

[J03] 字符串解析为日期
来源：http://uyr.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zql.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wyi.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://xip.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://sqb.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qpo.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wtb.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://mtx.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dnr.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://pya.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pyp.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vpq.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vbd.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jox.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rhe.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ofq.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eul.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nwl.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://csi.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://kxq.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gyd.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzc.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jxm.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://ihd.sysykeji.top


<!-- 参考信息 -->