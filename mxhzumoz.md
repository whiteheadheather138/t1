代发 wailian999

TS:   public / protected / private
来源：http://bxd.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://jxx.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iih.bbcook.cn

Ruby: public / protected / private
来源：http://tlq.yueranfly.top

C#:   public / protected / private / internal
来源：http://whp.birdmap.top

[G11] getter / setter
来源：http://rwm.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://psh.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cbo.hesvh.cn

JS:   get name() { return this._name; }
来源：http://lyc.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://dqq.gotoacloud.top

Java: public String getName() { return name; }
来源：http://yet.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bbn.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://uka.yueranfly.top

C#:   public string Name { get; set; }
来源：http://zyu.fengsongda.top

[G12] 对象转字符串
来源：http://bsp.birdmap.top

Py:   def __str__(self): return self.name
来源：http://mdn.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dxs.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://niq.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://qio.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://klt.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pth.andypj.xyz

Ruby: def to_s; @name; end
来源：http://kqj.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://gis.fengsongda.top

[G13] 判断对象类型
来源：http://vkf.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://hqu.xziqi.cn

PHP:  $u instanceof User
来源：http://qux.guannengcc.top

JS:   u instanceof User
来源：http://gmt.yfazqb.com

TS:   u instanceof User
来源：http://pul.iojbl.cn

Java: u instanceof User
来源：http://xmk.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ucd.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://jyv.iojbl.cn

C#:   u is User
来源：http://reb.dashuyun.cn

[G14] 数据类 / record
来源：http://spw.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://faj.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://tie.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://ysa.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://lqt.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://kxx.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://xsg.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zjr.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://dvz.yj20258888.top

[G15] 枚举
来源：http://dsv.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mhl.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jxg.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aeq.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lka.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://kht.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rgv.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://olo.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zxl.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://zil.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oen.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://wfz.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://yhh.gzhubu.top

TS:   Object.entries(obj)
来源：http://mpr.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bro.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dzo.smart0.xyz

Ruby: obj.instance_variables
来源：http://zql.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://njb.shuidangran.top

================================================================================
来源：http://buq.fengsongda.top

H. 异常与错误处理
来源：http://wnr.tianlin.xyz

================================================================================
来源：http://jmk.zycfv.cn

[H01] try / catch 基础
来源：http://ptv.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ewa.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nxi.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rxa.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hfl.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://idi.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zck.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dec.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tbb.fzhhl.top

[H02] finally / ensure 收尾
来源：http://qsb.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://dkz.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zfo.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jkg.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zwe.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kfz.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jjv.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kfl.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bej.tanke756.top

[H03] 主动抛出异常
来源：http://jme.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://pdr.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vlz.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://roi.yj20258.top

TS:   throw new Error("错误信息");
来源：http://aha.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tvw.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fwx.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://usr.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://ceh.yongpay.top

[H04] 自定义异常类型
来源：http://uit.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://nds.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://cxf.hnqzz.top

JS:   class MyError extends Error {}
来源：http://qxg.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://ecr.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://phj.316326.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ckj.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://dqr.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://naq.yangfankeji.com

[H05] 捕获特定类型
来源：http://czx.uphjek.com

Py:   except ValueError as e:
来源：http://ivr.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pee.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://erq.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://rig.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://bku.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qmv.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://bvo.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vkg.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://slj.sweek.top

Py:   value = d.get("k") or default
来源：http://tmc.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://atl.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://pen.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rcs.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cwz.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://amj.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://ort.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://rsg.tanke756.top

[H07] 断言
来源：http://aue.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://ryq.jyoumei.cn

PHP:  assert($x > 0);
来源：http://yto.yvedp.cn

JS:   console.assert(x > 0);
来源：http://ism.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://jal.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://bcz.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jgo.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://gok.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://rth.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://lgs.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://lum.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vxu.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://wzj.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://okd.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ajb.chenlongwang.top

Go:   err.Error()
来源：http://hjq.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://ofi.shanyushiyangtech.top

C#:   e.Message;  e.StackTrace
来源：http://zlq.xziqi.cn

[H09] 带错误码的异常
来源：http://kqa.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vao.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pkn.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ffx.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yyu.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yby.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tdw.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vhu.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://shp.vqdsnc.cn

[H10] 资源自动释放
来源：http://rkf.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://hqy.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ggj.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://znc.epnwcf.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://glw.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ybs.bbcook.cn

Go:   defer f.Close()
来源：http://ttv.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mtg.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ste.cashguo.top

================================================================================
来源：http://rro.yanxiufei.cn

I. 正则表达式
来源：http://rzp.jinqigufen.top

================================================================================
来源：http://zaa.gogol.net.cn

[I01] 判断是否匹配
来源：http://qdq.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cip.jqgfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://llt.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://zwq.yj20258.top

TS:   /\d+/.test(s)
来源：http://nqq.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://huj.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lbl.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://tru.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://phu.yj202588.top

[I02] 提取所有匹配
来源：http://usg.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://hxp.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://krw.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vhe.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://vcf.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sib.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cvp.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://vsv.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://drf.ydzc1.top

[I03] 提取捕获分组
来源：http://nqq.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ney.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rkn.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tqi.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://scq.fehbvm.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zvw.ivvv.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://isf.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ofu.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dqh.hesvh.cn

[I04] 正则替换
来源：http://mad.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://njz.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kca.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kgj.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://naa.gogol.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oij.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dii.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fkc.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ybb.uphjek.com

[I05] 按正则拆分
来源：http://frs.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://utx.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qvg.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://hpx.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://vpo.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://epq.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ott.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hem.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tqw.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://srf.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://evv.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qwv.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ped.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bgk.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dcf.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kbn.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xgr.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rno.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://ybn.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zsn.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sko.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kex.hesvh.cn

TS:   /error/gim
来源：http://nsw.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vgw.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tlf.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://mbd.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zcc.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://tzx.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rwi.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qba.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yxq.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dqg.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jls.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://edc.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://voa.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tye.jinqigfzy.top

================================================================================
来源：http://tsp.ybcxt.top

J. 日期与时间
来源：http://fdn.wangdashe.top

================================================================================
来源：http://tyx.0kj1m.cn

[J01] 获取当前时间
来源：http://coh.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wok.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uja.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://vds.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://nnj.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vic.shuidangran.top

Go:   time.Now()
来源：http://ukd.jyoumei.cn

Ruby: Time.now
来源：http://mru.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fmq.hywenlv.cn

[J02] 格式化输出
来源：http://yrz.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pmo.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ket.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eqr.pycfn.com

TS:   d.toISOString()
来源：http://fco.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aws.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iyp.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qyg.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tpk.jyoumei.cn

[J03] 字符串解析为日期
来源：http://pqf.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vex.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pcb.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://kct.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://mlv.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://toe.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blh.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://syl.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://txg.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://mew.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rqy.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ccz.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mcs.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uns.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://myp.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jcf.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vvb.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mqf.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://sys.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://dam.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mxx.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://esp.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xge.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://hwh.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nyn.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://oio.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://tnp.hysaishi.cn

[J06] 计算两时间之差
来源：http://nwy.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://ify.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://sht.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sbl.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kio.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://zgh.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://ueu.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://anp.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://syc.daxiang520.top

[J07] 比较两个日期
来源：http://bqj.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://hgy.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sto.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://pmg.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://vxe.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lpd.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ssh.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://byu.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://yiz.redwolf501.top

[J08] 提取年月日与星期
来源：http://rmb.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bzb.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dlk.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kkb.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tpa.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sbb.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tdi.xziqi.cn


<!-- 参考信息 -->