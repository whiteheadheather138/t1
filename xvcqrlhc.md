代发 wailian999

JS:   super.greet();
来源：http://eht.vqdsnc.cn

TS:   super.greet();
来源：http://gmr.birdmap.top

Java: super.greet();
来源：http://syb.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tbu.dashuyun.cn

Ruby: super
来源：http://kcw.iojbl.cn

C#:   base.Greet();
来源：http://xdv.epnwcf.com

[G08] 静态方法与属性
来源：http://wfw.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wbi.vehdjk.com

PHP:  public static function f() {}
来源：http://bjd.xuanzx.com

JS:   static f() {}
来源：http://hio.feifeiyinyue.top

TS:   static f(): void {}
来源：http://uhj.yanxiufei.cn

Java: static void f() {}
来源：http://ztp.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bow.birdmap.top

Ruby: def self.f; end
来源：http://jzm.zhixingplan.top

C#:   public static void F() {}
来源：http://qwk.birdmap.top

[G09] 接口 / 抽象类
来源：http://eqf.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://ikq.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pnu.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qst.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://spe.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://elf.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://jld.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sso.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://gtt.chenjidiqi.icu

[G10] 访问控制
来源：http://zjy.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://gty.zhiwuduotai.top

PHP:  public / protected / private
来源：http://nvd.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://imd.nwbrower.top

TS:   public / protected / private
来源：http://zez.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://drh.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://jzr.xinyue.icu

Ruby: public / protected / private
来源：http://txd.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://yph.xinyue.icu

[G11] getter / setter
来源：http://ssn.fktsv.cn

Py:   @property 与 @x.setter
来源：http://tlh.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lbo.cucudq.cn

JS:   get name() { return this._name; }
来源：http://ecq.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://xlt.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://uts.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bho.yj20258888.top

Ruby: attr_accessor :name
来源：http://dwo.ydzc1.top

C#:   public string Name { get; set; }
来源：http://qnm.52xcode.cn

[G12] 对象转字符串
来源：http://xdz.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://ixq.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dwn.yj20258888.top

JS:   toString() { return this.name; }
来源：http://amp.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://dlm.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://qtl.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://dvw.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://nyp.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://rll.shuidangran.top

[G13] 判断对象类型
来源：http://bnm.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://nrv.vehdjk.com

PHP:  $u instanceof User
来源：http://oaf.cashguo.top

JS:   u instanceof User
来源：http://chj.hysaishi.cn

TS:   u instanceof User
来源：http://mkm.meibo888.top

Java: u instanceof User
来源：http://ojv.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lmc.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://uzu.sufxvd.cn

C#:   u is User
来源：http://jpc.hcnkem.com

[G14] 数据类 / record
来源：http://gpm.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ick.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://pow.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://nar.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://zqn.birdmap.top

Java: record User(String name, int age) {}
来源：http://hcb.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://asf.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xmz.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://dek.shanyushiyangtech.top

[G15] 枚举
来源：http://jwi.gogol.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://khy.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://isz.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bxm.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jqx.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://kzl.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://skm.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://pkj.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mxa.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://dbb.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zud.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://zfe.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://zmz.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://bvz.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fma.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hqu.guannengcc.top

Ruby: obj.instance_variables
来源：http://vhv.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://xig.hcnkem.com

================================================================================
来源：http://icw.cheryme.top

H. 异常与错误处理
来源：http://hko.jqgufenzy.top

================================================================================
来源：http://azv.haohaochexian.top

[H01] try / catch 基础
来源：http://iul.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fei.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kto.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tza.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pby.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gjk.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uuw.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vwx.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mzt.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://rbt.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hto.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gdz.hnqzz.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pbd.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sne.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://doh.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mgb.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://qfb.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dcj.uphjek.com

[H03] 主动抛出异常
来源：http://qko.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://lei.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://urf.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://cfc.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://ung.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pip.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sfs.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vfe.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bdj.yj202588.top

[H04] 自定义异常类型
来源：http://xer.uphjek.com

Py:   class MyError(Exception): pass
来源：http://hsu.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://ign.redwolf501.top

JS:   class MyError extends Error {}
来源：http://igx.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://uxl.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://whc.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bch.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://ulj.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://fxw.hesvh.cn

[H05] 捕获特定类型
来源：http://dok.andypj.xyz

Py:   except ValueError as e:
来源：http://vow.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tub.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://yhw.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://hwr.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://slz.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vav.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://mmv.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wcv.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://ybk.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://idc.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jjr.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://yvi.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nlw.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dtq.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wlm.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://drh.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://onn.xuetiantiany.cn

[H07] 断言
来源：http://dwh.jqgufenzy.top

Py:   assert x > 0, "必须为正"
来源：http://sii.aibaodan.cn

PHP:  assert($x > 0);
来源：http://pwq.andypj.xyz

JS:   console.assert(x > 0);
来源：http://ack.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://bej.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://ejn.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://awh.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ifv.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://sxu.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://fbj.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://ahb.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zhr.svipenyu.cn

JS:   e.message;  e.stack
来源：http://pkt.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://irj.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ksl.fzhhl.top

Go:   err.Error()
来源：http://awd.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://kyi.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://emi.9152youxi.cn

[H09] 带错误码的异常
来源：http://fdg.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fpz.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lzi.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qxz.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jcm.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mcg.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gxt.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://ayp.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://azc.yj20258.top

[H10] 资源自动释放
来源：http://pjy.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://axm.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qbh.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ecg.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nup.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uqx.jqgufenzy.top

Go:   defer f.Close()
来源：http://tap.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aus.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zgj.hcnkem.com

================================================================================
来源：http://ewr.yfazqb.com

I. 正则表达式
来源：http://poq.aibaodan.cn

================================================================================
来源：http://qsn.sweek.top

[I01] 判断是否匹配
来源：http://ofd.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mvy.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uip.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://ljn.daria6918.cn

TS:   /\d+/.test(s)
来源：http://ghd.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cpo.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qzw.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://pjj.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hzk.jyoumei.cn

[I02] 提取所有匹配
来源：http://skh.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://lrk.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ymq.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://usz.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://lwh.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gdx.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://txs.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://ecp.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ypc.tarul.cn

[I03] 提取捕获分组
来源：http://pea.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://okc.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tnt.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zuq.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wqy.shanyushiyangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bsf.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xbm.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://upl.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eql.snrcjt.cn

[I04] 正则替换
来源：http://orr.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://qmh.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lkm.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://vlm.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://hpe.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://tnk.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://qqk.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wgq.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://joi.svipenyu.cn

[I05] 按正则拆分
来源：http://pvi.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://szj.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uhz.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://dpg.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://ehy.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://nyf.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qgz.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rvx.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xqn.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yis.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://epi.ydjk.org.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ifj.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zsz.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dnj.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rdt.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vfy.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kbf.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://klh.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://kvz.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ahb.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rxt.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lbu.svipenyu.cn

TS:   /error/gim
来源：http://ygv.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aiz.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://boq.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://ado.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rjt.shanyushiyangtech.top

[I08] 贪婪与非贪婪匹配
来源：http://qoz.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tlq.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dtt.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fob.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vmo.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sdh.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ejv.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aav.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ote.wangdashe.top

================================================================================
来源：http://wee.yanxiufei.cn

J. 日期与时间
来源：http://qcg.wangdashe.top

================================================================================
来源：http://elp.guannengcc.top

[J01] 获取当前时间
来源：http://mva.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xrj.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sqp.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://ghb.fengsongda.top

TS:   new Date();  Date.now()
来源：http://jzu.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kgd.yanxiufei.cn

Go:   time.Now()
来源：http://mjv.zdbjq.cn

Ruby: Time.now
来源：http://qhe.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zsj.zycfv.cn

[J02] 格式化输出
来源：http://olv.bbcook.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ogt.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://csw.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rpe.jqgfzy.top

TS:   d.toISOString()
来源：http://nyo.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sjj.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qjb.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ziq.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dtn.tian-w.cn

[J03] 字符串解析为日期
来源：http://ilu.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zpq.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pkr.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://pvg.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://rjq.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ymm.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gol.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://eis.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://khd.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://iqj.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yny.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sev.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xre.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gaq.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yjk.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rrq.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qpp.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mxl.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://ete.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://bmw.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bft.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pwk.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eiz.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://msa.hcnkem.com


<!-- 参考信息 -->