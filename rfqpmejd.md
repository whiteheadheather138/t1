代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://nsj.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://vxi.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ufn.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://lai.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://ajg.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://uid.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lbx.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://dlt.jlsjyb.cn

[G10] 访问控制
来源：http://lfx.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://fva.hnxiangtu.top

PHP:  public / protected / private
来源：http://yhf.yj20258888.top

JS:   #private 字段；其余公开
来源：http://arp.hesvh.cn

TS:   public / protected / private
来源：http://iui.pycfn.com

Java: public / protected / private / 默认包级
来源：http://abu.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bnk.andypj.xyz

Ruby: public / protected / private
来源：http://yic.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://ljj.fzhhl.top

[G11] getter / setter
来源：http://hwq.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://qsn.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kvd.hfpthk.cn

JS:   get name() { return this._name; }
来源：http://svr.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://xrd.zdqjudy.top

Java: public String getName() { return name; }
来源：http://ozn.xinyue.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://lyw.9152youxi.cn

Ruby: attr_accessor :name
来源：http://mem.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://jho.tarul.cn

[G12] 对象转字符串
来源：http://yrv.sweek.top

Py:   def __str__(self): return self.name
来源：http://qcj.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kwo.hesvh.cn

JS:   toString() { return this.name; }
来源：http://akb.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://pis.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://cmr.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bda.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://nbx.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://sre.316326.xyz

[G13] 判断对象类型
来源：http://itk.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://afk.yueranfly.top

PHP:  $u instanceof User
来源：http://yxo.zhiwuduotai.top

JS:   u instanceof User
来源：http://ijy.nwbrower.top

TS:   u instanceof User
来源：http://sev.yueranfly.top

Java: u instanceof User
来源：http://cox.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://crp.c1oappe.top

Ruby: u.is_a?(User)
来源：http://tvf.yonumen.top

C#:   u is User
来源：http://msk.bbcook.cn

[G14] 数据类 / record
来源：http://bjw.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://roy.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://itw.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://xmo.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://hxc.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://zlk.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://ddf.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xjw.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://pcb.yj20258.top

[G15] 枚举
来源：http://hev.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zfm.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bis.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nwi.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fzj.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://xlk.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rym.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://spk.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vxv.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://ock.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://peq.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://vbm.meibo888.top

JS:   Object.entries(obj)
来源：http://klk.jinqigufen.top

TS:   Object.entries(obj)
来源：http://ulq.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zai.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vmt.cqqwz.cn

Ruby: obj.instance_variables
来源：http://aaz.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://wzr.epnwcf.com

================================================================================
来源：http://qxt.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://ryg.xuanzx.com

================================================================================
来源：http://yhl.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://mly.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jmx.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dsn.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zdh.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rqv.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://has.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kmr.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://efp.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ptx.yj20258.top

[H02] finally / ensure 收尾
来源：http://kal.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://kho.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://uda.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://esn.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mha.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://tki.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sxf.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uyl.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dpt.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://isz.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://kzm.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mos.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://hip.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://ppu.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ahx.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gdg.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fuk.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://hol.xuanzx.com

[H04] 自定义异常类型
来源：http://yrj.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://iyq.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://yax.bbcook.cn

JS:   class MyError extends Error {}
来源：http://evk.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://eec.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://dzz.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fms.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://qej.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://shs.sweek.top

[H05] 捕获特定类型
来源：http://uxq.hammf.cn

Py:   except ValueError as e:
来源：http://aup.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ost.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://gkt.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://rfp.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://qzx.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wsj.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://ksm.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pkb.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://vgj.ydzc1.top

Py:   value = d.get("k") or default
来源：http://ing.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dvt.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zai.zhoulong.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://waz.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rna.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hxm.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://cam.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://enr.hysaishi.cn

[H07] 断言
来源：http://ulw.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://jzh.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://gdr.tianlin.xyz

JS:   console.assert(x > 0);
来源：http://upg.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://uww.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://dag.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tlw.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dus.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://uwu.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://ojn.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://qmi.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oey.yonumen.top

JS:   e.message;  e.stack
来源：http://jet.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fuc.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://vjo.quarkkingdee.top

Go:   err.Error()
来源：http://ugy.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://gom.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://azy.hammf.cn

[H09] 带错误码的异常
来源：http://led.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://crn.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://qnl.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kuo.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xqw.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fpc.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nbr.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tlg.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tse.sufxvd.cn

[H10] 资源自动释放
来源：http://ebv.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lor.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tdz.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hyq.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nbn.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jkf.havefunace.top

Go:   defer f.Close()
来源：http://bnu.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zwy.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vvj.vqdsnc.cn

================================================================================
来源：http://acn.hywenlv.cn

I. 正则表达式
来源：http://gbt.yj20258888.top

================================================================================
来源：http://dir.jiagoushi.top

[I01] 判断是否匹配
来源：http://ryd.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://orv.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ykp.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://rzo.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://yfy.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ukr.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jrm.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://vff.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jum.sufxvd.cn

[I02] 提取所有匹配
来源：http://bwu.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://acs.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mju.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jrf.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://wwj.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gmh.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qjk.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://ycc.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mko.zdbjq.cn

[I03] 提取捕获分组
来源：http://sds.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gbp.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://irh.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hgk.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zkk.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ldz.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fja.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zbj.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uyr.snrcjt.cn

[I04] 正则替换
来源：http://meg.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eqi.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nye.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://gnj.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zdq.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://wec.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dqy.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dpb.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uwt.nanxinkj.top

[I05] 按正则拆分
来源：http://lyc.zdqjudy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ael.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://glh.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://onj.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://lyf.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://nqm.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yoq.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://psy.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hmk.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://owx.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fnb.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zya.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zyc.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msi.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fvm.xylfe.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://taa.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://goc.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mey.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://lyw.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://icv.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vun.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bea.hfpthk.cn

TS:   /error/gim
来源：http://wey.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uap.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uga.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://cli.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ltb.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://mug.nanxinkj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mms.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sen.sufxvd.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hqx.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ygo.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tpx.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jru.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gpc.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sfp.hcnkem.com

================================================================================
来源：http://ide.zdqjudy.top

J. 日期与时间
来源：http://grn.wangshuangyany.cn

================================================================================
来源：http://qfz.redwolf501.top

[J01] 获取当前时间
来源：http://xdq.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oeb.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bkk.daria6918.cn

JS:   new Date();  Date.now()
来源：http://usd.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://hpl.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lfk.xinyue.icu

Go:   time.Now()
来源：http://slk.haohaochexian.top

Ruby: Time.now
来源：http://hkn.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wkh.hnqzz.top

[J02] 格式化输出
来源：http://spd.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cil.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jiq.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://frk.xuanzx.com

TS:   d.toISOString()
来源：http://tkw.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yee.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xnt.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kss.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sft.cucudq.cn

[J03] 字符串解析为日期
来源：http://ier.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zxb.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zln.sweek.top

JS:   new Date("2024-01-02")
来源：http://kxm.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://jxj.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://hwp.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dfo.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://psi.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sgb.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://nqo.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://urg.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://syf.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zwb.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dex.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cpz.fanxiaobao.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zfv.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kpc.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mts.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://vds.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://nbb.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cwa.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eej.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yte.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://aiv.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uza.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://uug.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://agb.xylfe.cn

[J06] 计算两时间之差
来源：http://sqp.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://jpr.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://gru.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ach.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wbr.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fvb.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://kxe.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://lpc.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://zzd.316326.xyz

[J07] 比较两个日期
来源：http://gyv.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://hey.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nzr.cdnleiting.top

JS:   d1.getTime() < d2.getTime()
来源：http://ttk.ydzc1.top


<!-- 参考信息 -->