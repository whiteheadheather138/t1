代发 wailian999

[G10] 访问控制
来源：http://rld.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://edc.shzxlz.cn

PHP:  public / protected / private
来源：http://iqj.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://fox.jinqigufen.top

TS:   public / protected / private
来源：http://nkr.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://xbd.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aza.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://sja.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://tlh.gaohongyu789.top

[G11] getter / setter
来源：http://rqe.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://otn.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bjs.ydzc1.top

JS:   get name() { return this._name; }
来源：http://frc.zdqjudy.top

TS:   get name(): string { return this._name; }
来源：http://gyb.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://vrx.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://mwb.yongpay.top

Ruby: attr_accessor :name
来源：http://jpg.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://dtr.aibaodan.cn

[G12] 对象转字符串
来源：http://qqh.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://ujl.hcnkem.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://hch.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://gvc.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://fgj.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://erm.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zgi.fehbvm.com

Ruby: def to_s; @name; end
来源：http://atk.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://nps.uphjek.com

[G13] 判断对象类型
来源：http://dai.iojbl.cn

Py:   isinstance(u, User)
来源：http://xvw.fktsv.cn

PHP:  $u instanceof User
来源：http://cuy.zhoulong.xyz

JS:   u instanceof User
来源：http://vik.pycfn.com

TS:   u instanceof User
来源：http://dmx.zdqjudy.top

Java: u instanceof User
来源：http://wsd.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rkn.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://zrm.mhx1999.top

C#:   u is User
来源：http://hno.zhongyouzk.top

[G14] 数据类 / record
来源：http://foz.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://phl.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://sdh.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://fni.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://mmj.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://tyo.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://irr.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gbv.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://ske.xylfe.cn

[G15] 枚举
来源：http://gta.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wxv.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dfj.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ife.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://daf.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://wva.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rwi.hysaishi.cn

Ruby: Color = %i[red green].freeze
来源：http://egc.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://egl.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://fsg.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dip.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://hbm.hesvh.cn

JS:   Object.entries(obj)
来源：http://zqx.haohaochexian.top

TS:   Object.entries(obj)
来源：http://jhe.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gph.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://udk.svipenyu.cn

Ruby: obj.instance_variables
来源：http://qzo.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://akw.zhongyouzk.top

================================================================================
来源：http://nff.ydjk.org.cn

H. 异常与错误处理
来源：http://esa.ppjwa.cn

================================================================================
来源：http://agx.jyoumei.cn

[H01] try / catch 基础
来源：http://hwi.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fwa.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bqs.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cxp.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rww.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ovr.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://une.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nmv.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qoa.bbcook.cn

[H02] finally / ensure 收尾
来源：http://dxt.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://fby.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zee.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gof.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xuq.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://qcs.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cqw.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://olj.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hvx.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://pam.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://fcn.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tmw.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://ghn.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://buv.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cxz.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://luu.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://btl.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://lnc.quarkkingdee.top

[H04] 自定义异常类型
来源：http://efs.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://vjp.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://jsl.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://icu.birdmap.top

TS:   class MyError extends Error {}
来源：http://ewn.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://emz.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jvq.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://thd.yuxming.cn

C#:   class MyException : Exception {}
来源：http://nqs.zhongyouzk.top

[H05] 捕获特定类型
来源：http://qob.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://etq.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rhr.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://sfn.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://zlk.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://aog.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lch.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://dhs.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://spx.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://yje.yj202588.top

Py:   value = d.get("k") or default
来源：http://wlm.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wsa.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://gjf.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://ogv.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nvr.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qeu.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://hum.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://bvh.c1oappe.top

[H07] 断言
来源：http://uyn.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://kvv.zdbjq.cn

PHP:  assert($x > 0);
来源：http://nvu.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://val.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://psp.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://jko.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eco.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://sbd.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://jss.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://afp.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://ceb.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iir.vehdjk.com

JS:   e.message;  e.stack
来源：http://imk.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hyc.jinqigfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cbl.ywan-chungtsiang.top

Go:   err.Error()
来源：http://esj.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://rus.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://ehs.daxiang520.top

[H09] 带错误码的异常
来源：http://yuz.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gre.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://urp.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rht.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yrx.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xyv.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hdp.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://hjc.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fib.ivvv.top

[H10] 资源自动释放
来源：http://fhc.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jkk.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://frh.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jwx.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xgn.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dag.jiagoushi.top

Go:   defer f.Close()
来源：http://piy.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tzs.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tfp.xuetiantiany.cn

================================================================================
来源：http://shc.fzhhl.top

I. 正则表达式
来源：http://wfd.yj20258888.top

================================================================================
来源：http://xto.tarul.cn

[I01] 判断是否匹配
来源：http://enx.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qmr.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://ajd.pycfn.com

JS:   /\d+/.test(s)
来源：http://yxx.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://mty.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vuz.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oat.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://ttw.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vkt.jiagoushi.top

[I02] 提取所有匹配
来源：http://wad.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://tbh.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dxv.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gqt.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://gee.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tmo.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ppt.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://ria.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hwo.jyoumei.cn

[I03] 提取捕获分组
来源：http://eob.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dxk.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yqe.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ykk.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cjz.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uuw.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mit.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rsa.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ejw.aizwys.cn

[I04] 正则替换
来源：http://icz.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://oxq.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sdo.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://vxn.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jwu.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://wgt.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://fkk.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ftm.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cne.tian-w.cn

[I05] 按正则拆分
来源：http://wns.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wnr.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eto.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://ewc.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://mxh.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://ofz.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jpm.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wlq.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rzc.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tob.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tya.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bdd.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lhj.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bvv.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://urd.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pld.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ehz.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sxd.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://oqf.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://etl.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oaq.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rqu.mhx1999.top

TS:   /error/gim
来源：http://imb.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nso.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nas.ybcxt.top

Ruby: s.scan(/error/i)
来源：http://lrs.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oka.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://ddp.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tsj.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cby.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://igz.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hiz.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sba.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mpn.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://npl.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iic.chenzaomai.com

================================================================================
来源：http://drf.guowangkeji.top

J. 日期与时间
来源：http://ifa.fanxiaobao.xyz

================================================================================
来源：http://aqq.9152youxi.cn

[J01] 获取当前时间
来源：http://szx.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://wtf.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oob.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://kew.yj202588.top

TS:   new Date();  Date.now()
来源：http://jfy.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rpv.aibaodan.cn

Go:   time.Now()
来源：http://xxn.hysaishi.cn

Ruby: Time.now
来源：http://mbi.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mkz.shuidangran.top

[J02] 格式化输出
来源：http://fkm.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqa.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://znn.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eim.mhx1999.top

TS:   d.toISOString()
来源：http://mzf.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://giw.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bzu.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://obs.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kxx.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://fmv.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://shd.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bsy.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://jhd.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://umu.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://ioc.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ies.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://ppm.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zxu.fengsongda.top

[J04] 时间戳与日期互转
来源：http://way.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lin.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pkp.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wua.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kgr.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mht.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lkd.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zty.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://huz.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://ydr.ivvv.top

Py:   now + timedelta(days=7)
来源：http://zwq.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://mdm.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fzl.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://axt.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://ysz.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kcg.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://dbs.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cud.sjlbkw.cn

[J06] 计算两时间之差
来源：http://syx.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://ofi.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://sdb.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bgg.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zxh.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://wwf.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://bqh.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://wjq.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://hvo.zhoulong.xyz

[J07] 比较两个日期
来源：http://cqb.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://sze.zhoulong.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lwo.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://soo.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://ivr.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nss.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nii.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lct.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://etb.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://cgd.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pnh.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ypf.shzxlz.cn


<!-- 参考信息 -->