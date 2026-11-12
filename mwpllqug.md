代发 wailian999

[G10] 访问控制
来源：http://own.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://dgk.cucudq.cn

PHP:  public / protected / private
来源：http://njr.nwbrower.top

JS:   #private 字段；其余公开
来源：http://rhp.316326.xyz

TS:   public / protected / private
来源：http://pnj.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://san.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://keo.meibo888.top

Ruby: public / protected / private
来源：http://afh.meibo888.top

C#:   public / protected / private / internal
来源：http://zod.hcnkem.com

[G11] getter / setter
来源：http://ouj.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://hsx.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ehr.yongpay.top

JS:   get name() { return this._name; }
来源：http://imv.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://kpk.yonumen.top

Java: public String getName() { return name; }
来源：http://lrv.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bqt.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://dqh.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://ely.meibo888.top

[G12] 对象转字符串
来源：http://nzn.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://ahj.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kwz.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://frr.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://tue.cdnleiting.top

Java: @Override public String toString() { return name; }
来源：http://saz.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://gce.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://vvv.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://lxd.sjlbkw.cn

[G13] 判断对象类型
来源：http://rxb.ydjk.org.cn

Py:   isinstance(u, User)
来源：http://pyu.shuidangran.top

PHP:  $u instanceof User
来源：http://cml.yanxiufei.cn

JS:   u instanceof User
来源：http://sln.gotoacloud.top

TS:   u instanceof User
来源：http://ncs.iojbl.cn

Java: u instanceof User
来源：http://hmj.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://shb.bbcook.cn

Ruby: u.is_a?(User)
来源：http://osh.bjfxy.top

C#:   u is User
来源：http://bmk.hammf.cn

[G14] 数据类 / record
来源：http://juy.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://psl.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://bte.sjlbkw.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ohd.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://omn.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://par.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://uhz.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nlu.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://bat.pengpengdd.cyou

[G15] 枚举
来源：http://niy.dashuyun.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://chs.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zje.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kja.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qar.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://xif.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tsx.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://pws.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zss.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://dkt.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pwk.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://pxr.nanxinkj.top

JS:   Object.entries(obj)
来源：http://tlk.dianchejie.cn

TS:   Object.entries(obj)
来源：http://xqc.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gxo.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dwr.bbcook.cn

Ruby: obj.instance_variables
来源：http://nam.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://hro.xingfuxueyuan.xyz

================================================================================
来源：http://jre.hcnkem.com

H. 异常与错误处理
来源：http://oqb.hfpthk.cn

================================================================================
来源：http://uxv.ppjwa.cn

[H01] try / catch 基础
来源：http://pds.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pni.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iur.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vos.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mjd.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gkt.jlsjyb.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nrb.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cfp.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uuc.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://slh.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://tow.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://wqr.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ogt.haohaochexian.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zye.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gvs.zhoulong.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://cto.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jys.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://coa.uphjek.com

[H03] 主动抛出异常
来源：http://jng.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://gvw.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eqo.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://wii.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://tsp.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://yti.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xir.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zdq.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://eif.xziqi.cn

[H04] 自定义异常类型
来源：http://kwm.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://dyh.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yyo.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://xxb.hnqzz.top

TS:   class MyError extends Error {}
来源：http://ndz.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://aqi.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eph.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://eyr.daria6918.cn

C#:   class MyException : Exception {}
来源：http://skx.fengsongda.top

[H05] 捕获特定类型
来源：http://aet.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://vld.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kca.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://zmk.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://emw.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://jhm.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zun.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://nmr.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kih.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://wnc.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://drj.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://jey.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://wtl.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tww.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pbr.wangshuangyany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sbb.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://qct.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://upc.daria6918.cn

[H07] 断言
来源：http://yne.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://wnt.yfazqb.com

PHP:  assert($x > 0);
来源：http://zrr.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://ikt.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://rfg.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://ccb.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jca.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://syp.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://wso.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://ggw.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://mlj.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aqx.jinqigufen.top

JS:   e.message;  e.stack
来源：http://dhw.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jxb.yuxming.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dfs.sweek.top

Go:   err.Error()
来源：http://bdo.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://uxw.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://fgv.hcnkem.com

[H09] 带错误码的异常
来源：http://iyi.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xgv.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lsb.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fbv.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://epn.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://srr.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uxl.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jtj.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dwf.gaohongyu789.top

[H10] 资源自动释放
来源：http://ckt.sjlbkw.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eep.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zpf.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ydx.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sbh.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aov.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://vao.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qrm.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hzj.316326.xyz

================================================================================
来源：http://kbb.vehdjk.com

I. 正则表达式
来源：http://hkt.sysykeji.top

================================================================================
来源：http://ask.cqqwz.cn

[I01] 判断是否匹配
来源：http://gih.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://atm.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://mbh.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://zoc.nwbrower.top

TS:   /\d+/.test(s)
来源：http://plf.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fqs.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fme.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://hgk.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://npi.bjfxy.top

[I02] 提取所有匹配
来源：http://niu.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://hvn.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://snk.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yyh.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://jqg.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jgu.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tgb.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://xhj.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aqg.0kj1m.cn

[I03] 提取捕获分组
来源：http://sjz.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vpu.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kkk.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tym.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zna.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vyk.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zlg.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kih.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gew.c1oappe.top

[I04] 正则替换
来源：http://pgn.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xpx.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rjv.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jqn.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cca.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://pxv.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bav.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rld.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lux.yuanzhike.top

[I05] 按正则拆分
来源：http://zdz.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tor.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://veh.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://ubn.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://wol.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://edt.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://elq.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://vsj.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://plu.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://syp.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://day.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xyz.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lip.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yuh.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cjr.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zuw.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ehq.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gir.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://ere.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vqr.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dtd.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bvo.fktsv.cn

TS:   /error/gim
来源：http://anc.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yhd.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tkq.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://tuc.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ojj.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://btv.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xpi.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://htr.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fjr.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zko.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bcu.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oya.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zdv.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bmw.vqdsnc.cn

================================================================================
来源：http://tnc.shuidangran.top

J. 日期与时间
来源：http://lfr.aizwys.cn

================================================================================
来源：http://kzb.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://yyi.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tlq.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://flo.smart0.xyz

JS:   new Date();  Date.now()
来源：http://bii.fktsv.cn

TS:   new Date();  Date.now()
来源：http://iic.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yry.feifeiyinyue.top

Go:   time.Now()
来源：http://cdm.meibo888.top

Ruby: Time.now
来源：http://zaq.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://avf.ybcxt.top

[J02] 格式化输出
来源：http://fbi.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jkg.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xlm.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ozs.ctjpmb.com

TS:   d.toISOString()
来源：http://ouq.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jkh.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dtg.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://auw.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mwe.sweek.top

[J03] 字符串解析为日期
来源：http://jpm.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hdf.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zgz.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://fcw.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://mhk.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://jer.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lzy.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://hgc.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hni.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://suy.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wro.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ewe.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sit.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://std.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yys.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ebd.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pcc.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pyi.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://tsq.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://urp.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ukt.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fsk.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pko.meibo888.top

Java: LocalDate.now().plusDays(7)
来源：http://aki.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hni.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://mrk.sxryk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://run.aibaodan.cn

[J06] 计算两时间之差
来源：http://gmy.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://iav.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://mop.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wmx.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gkr.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://uge.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://ybh.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://cvp.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://kzp.hywenlv.cn

[J07] 比较两个日期
来源：http://nyz.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://zho.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cej.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://twi.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://xga.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://guq.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wld.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://aeh.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://esb.sysykeji.top

[J08] 提取年月日与星期
来源：http://vwi.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xbl.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ims.bbcook.cn


<!-- 参考信息 -->