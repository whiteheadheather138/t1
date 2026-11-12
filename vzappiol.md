代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wcl.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://xcj.uphjek.com

C#:   public static void F() {}
来源：http://ufj.fehbvm.com

[G09] 接口 / 抽象类
来源：http://qlf.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://kua.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://mgm.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lgy.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://zjq.ydzc1.top

Java: interface Shape { double area(); }
来源：http://iia.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://zxo.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nvn.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://poi.hcnkem.com

[G10] 访问控制
来源：http://qhm.ybcxt.top

Py:   约定 _protected / __private（不强制）
来源：http://zaf.daria6918.cn

PHP:  public / protected / private
来源：http://ggh.hcnkem.com

JS:   #private 字段；其余公开
来源：http://evv.shangyingyoupin.top

TS:   public / protected / private
来源：http://xgp.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://zci.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fqm.pengpengdd.cyou

Ruby: public / protected / private
来源：http://ktz.ctjpmb.com

C#:   public / protected / private / internal
来源：http://xti.yvedp.cn

[G11] getter / setter
来源：http://yzb.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://otp.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://sem.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://kok.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://cdo.fehbvm.com

Java: public String getName() { return name; }
来源：http://ndw.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xtm.yonumen.top

Ruby: attr_accessor :name
来源：http://dam.redwolf501.top

C#:   public string Name { get; set; }
来源：http://azj.gogol.net.cn

[G12] 对象转字符串
来源：http://bss.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://ynv.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yfb.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://uea.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://ayv.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://knb.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://avz.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://ezc.xinyue.icu

C#:   public override string ToString() => Name;
来源：http://lnr.wangshuangyany.cn

[G13] 判断对象类型
来源：http://ttg.jqgfzy.top

Py:   isinstance(u, User)
来源：http://nbb.sysykeji.top

PHP:  $u instanceof User
来源：http://eon.yonumen.top

JS:   u instanceof User
来源：http://efb.hnqzz.top

TS:   u instanceof User
来源：http://bkf.dashuyun.cn

Java: u instanceof User
来源：http://qff.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rcu.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://bts.fengsongda.top

C#:   u is User
来源：http://svj.ehwqpu.com

[G14] 数据类 / record
来源：http://hxt.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cya.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://nsy.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://zfj.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://led.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://yrh.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://gmo.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vam.yanxiufei.cn

C#:   record User(string Name, int Age);
来源：http://gxc.ybcxt.top

[G15] 枚举
来源：http://zkl.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dng.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jgg.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mrd.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://osq.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://epo.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hsr.cashguo.top

Ruby: Color = %i[red green].freeze
来源：http://ekl.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wrr.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://tmq.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nvw.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://sdb.yuxming.cn

JS:   Object.entries(obj)
来源：http://xkk.mhx1999.top

TS:   Object.entries(obj)
来源：http://jbu.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xfj.dashuyun.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uwr.wangshuangyany.cn

Ruby: obj.instance_variables
来源：http://hut.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://hil.bjfxy.top

================================================================================
来源：http://pqb.zhijiandao.cn

H. 异常与错误处理
来源：http://ekq.jinyuanbaomall.cn

================================================================================
来源：http://ywj.zdbjq.cn

[H01] try / catch 基础
来源：http://ktv.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bvj.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blu.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://izw.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nqh.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vot.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pww.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hmr.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kiu.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://pil.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://sqb.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://naw.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pvt.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wmk.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://oxl.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ioc.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://urc.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pdq.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://roe.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://ziu.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cno.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://xem.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://dgd.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ryn.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yck.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hqy.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wvj.epnwcf.com

[H04] 自定义异常类型
来源：http://vwb.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://lsi.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qah.yueranfly.top

JS:   class MyError extends Error {}
来源：http://wer.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://nam.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://ffo.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yas.tanke756.top

Ruby: class MyError < StandardError; end
来源：http://oyh.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://aau.uphjek.com

[H05] 捕获特定类型
来源：http://jje.yueranfly.top

Py:   except ValueError as e:
来源：http://ibg.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dnv.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://nxi.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://msy.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://xjk.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wok.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://ttn.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://acr.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://evt.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://igu.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://fvk.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mer.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://ngh.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xox.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://prs.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://oil.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://uun.zhoulong.xyz

[H07] 断言
来源：http://ujm.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://waa.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://fxk.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://ape.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://kkb.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://bqy.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ret.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://ppm.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://jnv.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://yjb.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://gao.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://djc.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://ajg.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://wtx.ybcxt.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ohm.daxiang520.top

Go:   err.Error()
来源：http://tli.redwolf501.top

Ruby: e.message;  e.backtrace
来源：http://mty.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://xzy.uphjek.com

[H09] 带错误码的异常
来源：http://sla.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://owv.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pqs.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gfa.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://snp.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nhi.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bic.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://vhc.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ury.jinqigufen.top

[H10] 资源自动释放
来源：http://sym.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xeo.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hjz.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nry.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yqo.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://con.kuanghao11.cn

Go:   defer f.Close()
来源：http://tkr.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ujx.zhiwuduotai.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dcu.jinghuilouyu.cn

================================================================================
来源：http://obq.smart0.xyz

I. 正则表达式
来源：http://baz.nanxinkj.top

================================================================================
来源：http://dal.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://tkz.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pry.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://kqe.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://qiu.tanke756.top

TS:   /\d+/.test(s)
来源：http://tgj.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wym.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oko.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://xsm.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kxo.ctjpmb.com

[I02] 提取所有匹配
来源：http://zxj.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://kxy.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gie.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hew.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://cre.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kwa.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://olu.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://qni.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ykk.vehdjk.com

[I03] 提取捕获分组
来源：http://dxq.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vwx.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pxi.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ekb.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zmc.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rsp.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xsp.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://spo.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mzk.snrcjt.cn

[I04] 正则替换
来源：http://xeg.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uhr.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jjx.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://maj.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://zrf.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://swu.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bid.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://zpj.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cbb.yfazqb.com

[I05] 按正则拆分
来源：http://jyf.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uwj.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dnt.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://mgb.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://khm.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://vbf.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vor.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://hxq.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lit.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bvw.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jqm.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uec.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dfg.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ofh.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ssd.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xsk.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tod.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ulr.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://jmb.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://njs.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pnf.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://olx.birdmap.top

TS:   /error/gim
来源：http://hjy.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kgj.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cdf.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://cxt.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vxy.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://wrx.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://swh.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eyp.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgq.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ukk.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://htn.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hem.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://clv.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vxu.nanxinkj.top

================================================================================
来源：http://xdi.tian-w.cn

J. 日期与时间
来源：http://kim.vqdsnc.cn

================================================================================
来源：http://lie.svipenyu.cn

[J01] 获取当前时间
来源：http://fif.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sua.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://otn.yvedp.cn

JS:   new Date();  Date.now()
来源：http://ofd.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://fzm.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qjt.daria6918.cn

Go:   time.Now()
来源：http://wzg.zhoulong.xyz

Ruby: Time.now
来源：http://mgs.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qfj.hnqzz.top

[J02] 格式化输出
来源：http://xgb.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxm.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gqf.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vkr.yuxming.cn

TS:   d.toISOString()
来源：http://ohx.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jdi.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yuj.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlq.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://izi.hfpthk.cn

[J03] 字符串解析为日期
来源：http://hsf.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hwq.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ysx.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://jfr.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://zcr.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://wtf.chenjidiqi.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uko.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://ywm.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://unk.daxiang520.top

[J04] 时间戳与日期互转
来源：http://xzb.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dmo.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://twr.hongshengwenyu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vke.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tys.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gwi.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bgb.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jyo.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qxz.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://pdj.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://rix.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ecj.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ijv.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sno.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://jlo.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iuw.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://nyf.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://sjz.zhixingplan.top

[J06] 计算两时间之差
来源：http://nzu.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://rpj.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://kdi.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mzp.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tuj.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://cyj.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://nhw.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://oad.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://pti.ppjwa.cn


<!-- 参考信息 -->