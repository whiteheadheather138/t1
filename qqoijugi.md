代发 wailian999

ANALYZE TABLE users;
来源：http://vqc.bjfxy.top

[Q71] 查看建表语句
来源：http://mqp.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ivr.xuetiantiany.cn

[Q72] 查看索引
来源：http://wyf.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://vfd.mhx1999.top

[Q73] 查看表状态
来源：http://jwh.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nzi.yanxiufei.cn

[Q74] 强制使用索引
来源：http://lbk.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://udf.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://plv.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bcs.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cly.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://zjb.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wwi.yangfankeji.com

[Q77] 时间加减
来源：http://gqx.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://stu.hfpthk.cn

[Q78] 当前时间
来源：http://kmu.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hmc.gzhubu.top

[Q79] 字符串拼接
来源：http://fjm.9152youxi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://svr.hesvh.cn

[Q80] 字符串截取
来源：http://zyi.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mra.havefunace.top

[Q81] 字符串替换
来源：http://hwn.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mkt.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://res.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tzd.birdmap.top

[Q83] 大小写转换
来源：http://eab.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://irb.yfazqb.com

[Q84] 去除首尾空格
来源：http://kgb.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://mly.wangshuangyany.cn

[Q85] 数值取整
来源：http://jmp.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vcv.tarul.cn

[Q86] 读取 JSON 字段
来源：http://wmn.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qsl.fengsongda.top

[Q87] JSON 字段做条件
来源：http://nzc.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dbr.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://psb.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ccv.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rhb.tarul.cn

[Q89] 判断表是否存在
来源：http://vms.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dtk.cashguo.top

[Q90] 生成序号列
来源：http://xli.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cog.zycfv.cn

================================================================================
来源：http://eax.tianlin.xyz

R. Bash 专题
来源：http://gcl.dianchejie.cn

================================================================================
来源：http://jwq.gogol.net.cn

[R01] shebang 与严格模式
来源：http://hmd.uphjek.com

#!/usr/bin/env bash
来源：http://caz.jlsjyb.cn

set -euo pipefail
来源：http://eeq.gzhubu.top

[R02] 变量赋值与使用
来源：http://qfj.birdmap.top

name="Tom"; echo "$name"
来源：http://jox.ehwqpu.com

[R03] 只读变量
来源：http://tyk.zhijiandao.cn

readonly PI=3.14
来源：http://qde.xuetiantiany.cn

[R04] 位置参数
来源：http://awz.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qxw.smart0.xyz

[R05] 参数默认值
来源：http://jgb.hesvh.cn

name="${1:-default}"
来源：http://hxv.wangdashe.top

[R06] 判断命令是否存在
来源：http://pbr.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zlm.havefunace.top

[R07] if 判断文件
来源：http://soo.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iju.zdbjq.cn

[R08] 数值比较
来源：http://dve.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uui.zdbjq.cn

[R09] 字符串比较
来源：http://lbp.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zqp.bjfxy.top

[R10] 正则匹配
来源：http://qfd.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wed.fanxiaobao.xyz

[R11] case 多分支
来源：http://yaz.ivvv.top

case "$1" in
来源：http://jih.nwbrower.top

start) echo "启动" ;;
来源：http://fwr.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://atu.guannengcc.top

*)     echo "未知命令" ;;
来源：http://kjb.zycfv.cn

esac
来源：http://yam.mhx1999.top

[R12] for 遍历文件
来源：http://izm.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://dxt.cashguo.top

[R13] for 计数循环
来源：http://ogz.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://mxn.yj202588.top

[R14] C 风格 for
来源：http://zpa.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zyb.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://pnz.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yvm.chenzaomai.com

[R16] until 等待条件
来源：http://xqj.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://buv.hammf.cn

[R17] 数组定义与取值
来源：http://lsa.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uom.haohaochexian.top

[R18] 遍历数组
来源：http://wjr.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://frd.tianlin.xyz

[R19] 数组长度
来源：http://ghb.sjlbkw.cn

echo "${#arr[@]}"
来源：http://zyd.jianghu66.top

[R20] 关联数组（字典）
来源：http://dff.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dma.jlsjyb.cn

[R21] 字符串长度
来源：http://yze.sysykeji.top

echo "${#s}"
来源：http://sku.fehbvm.com

[R22] 截取子串
来源：http://nit.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://xiv.kuanghao11.cn

[R23] 字符串替换
来源：http://huu.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dvs.tianlin.xyz

[R24] 大小写转换
来源：http://gtb.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://krr.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://man.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yth.pengpengdd.cyou

[R26] 命令替换
来源：http://yac.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://fpy.xylfe.cn

[R27] 算术展开
来源：http://rnl.redwolf501.top

echo $((1 + 2 * 3))
来源：http://wii.wangshuangyany.cn

[R28] 浮点运算
来源：http://uaf.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://lpm.zhiwuduotai.top

[R29] 定义函数
来源：http://icv.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://evf.hcnkem.com

[R30] 函数返回状态码
来源：http://vkx.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://yxk.pycfn.com

[R31] 局部变量
来源：http://qhl.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://nck.havefunace.top

[R32] 参数个数校验
来源：http://rvg.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yes.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://pkq.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oto.guowangkeji.top

[R34] 退出时清理
来源：http://qne.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nky.hywenlv.cn

[R35] 后台执行并等待
来源：http://stk.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://vfh.tarul.cn

[R36] 并发执行多个任务
来源：http://kuh.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gve.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://sej.shanyushiyangkeji.top

files=$(ls -1)
来源：http://lwa.yongpay.top

[R38] 管道串联
来源：http://hkc.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://poz.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://zji.hcnkem.com

cmd > out.log 2>&1
来源：http://yew.dashuyun.cn

[R40] 追加写日志
来源：http://yxm.xziqi.cn

echo "log" >> out.log
来源：http://jdt.tian-w.cn

[R41] 丢弃输出
来源：http://jwr.wangdashe.top

cmd >/dev/null 2>&1
来源：http://wpr.jyoumei.cn

[R42] 输入重定向
来源：http://hyk.pycfn.com

wc -l < a.txt
来源：http://lop.0kj1m.cn

[R43] 按名字查找文件
来源：http://uff.sweek.top

find . -name "*.log" -type f
来源：http://qse.yfazqb.com

[R44] 按修改时间查找
来源：http://jdc.dianchejie.cn

find . -mtime -7 -type f
来源：http://wmy.yueranfly.top

[R45] 批量删除
来源：http://tok.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://wcu.yj20258.top

[R46] 递归替换文件内容
来源：http://hjq.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jgp.xinyue.icu

[R47] sed 单行替换
来源：http://gfq.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tin.guowangkeji.top

[R48] awk 取指定列
来源：http://ntx.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://miz.guowangkeji.top

[R49] awk 带条件
来源：http://bdx.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xta.hongshengwenyu.top

[R50] awk 求和
来源：http://voh.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dog.zhijiandao.cn

[R51] 排序去重取前几
来源：http://haj.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://igl.ctjpmb.com

[R52] 统计行数
来源：http://tvo.andypj.xyz

wc -l a.txt
来源：http://quq.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://rvm.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jam.iojbl.cn

[R54] 比较两个文件
来源：http://yhn.zhijiandao.cn

diff a.txt b.txt
来源：http://cha.pycfn.com

[R55] 压缩与解压
来源：http://cpa.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kez.yangfankeji.com

[R56] 远程拷贝
来源：http://cgs.havefunace.top

scp file user@host:/path/
来源：http://grf.9152youxi.cn

[R57] 远程执行命令
来源：http://lzu.zdbjq.cn

ssh user@host 'uptime'
来源：http://ioz.epnwcf.com

[R58] 下载文件
来源：http://okr.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ujt.meibo888.top

[R59] 发 POST JSON
来源：http://kgp.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bzz.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://tfj.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wte.jinqigufen.top

[R61] 磁盘占用
来源：http://rtv.c1oappe.top

df -h;  du -sh *
来源：http://wdd.fehbvm.com

[R62] 找最占空间的文件
来源：http://wkt.fanxiaobao.xyz

du -ah . | sort -rh | head -10
来源：http://izo.jqgfzy.top

[R63] 内存与进程
来源：http://jah.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://yzi.vqdsnc.cn

[R64] 结束进程
来源：http://yyp.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://xtl.ydzc1.top

[R65] 查看端口占用
来源：http://qyb.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ixl.zhongyouzk.top

[R66] 定时任务
来源：http://nuj.svipenyu.cn

crontab -e;  crontab -l
来源：http://ito.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://ebd.fehbvm.com

openssl rand -hex 16
来源：http://avq.pycfn.com

[R68] 计算文件校验值
来源：http://orf.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://mwk.meibo888.top

[R69] 生成随机密码
来源：http://hxy.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://ljx.jyoumei.cn

[R70] 时间戳与互转
来源：http://mpd.yueranfly.top

date +%s;  date -d @1700000000
来源：http://wvk.daria6918.cn

[R71] 日期格式化
来源：http://rrm.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fyo.yongpay.top

[R72] 等待端口就绪
来源：http://vup.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sny.hcnkem.com

[R73] 分割大日志
来源：http://nro.0kj1m.cn

split -l 1000 big.log part_
来源：http://qtz.yonumen.top

[R74] 批量重命名
来源：http://fpt.ctjpmb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xba.andypj.xyz

[R75] 导出环境变量
来源：http://ahh.fengsongda.top

export PATH="$HOME/bin:$PATH"
来源：http://oea.bjfxy.top

[R76] 使用临时文件
来源：http://ubp.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ovm.daria6918.cn

[R77] 读取用户输入
来源：http://gtp.hnxiangtu.top

read -rp "请输入: " ans
来源：http://zjc.tanke756.top

[R78] 交互式菜单
来源：http://zqo.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://fxa.sysykeji.top

[R79] 解析命令行选项
来源：http://lsq.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://com.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://glf.ehwqpu.com

time ./run.sh
来源：http://zty.jinyuanbaomall.cn

================================================================================
来源：http://hap.zdqjudy.top

S. C / C++ 专题
来源：http://noh.uphjek.com

================================================================================
来源：http://ypz.chenjidiqi.icu

[S01] C：Hello World
来源：http://cem.nanxinkj.top

#include <stdio.h>
来源：http://ylu.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rtv.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://qns.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://zmq.cashguo.top

[S03] C：读入整数
来源：http://vwk.yongpay.top

int x; scanf("%d", &x);
来源：http://uml.cheryme.top

[S04] C：字符串复制
来源：http://hzc.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://cny.zhongyouzk.top

[S05] C：字符串长度
来源：http://yzk.jyoumei.cn

strlen(s)
来源：http://tvf.pycfn.com

[S06] C：字符串比较
来源：http://aix.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://mfx.cucudq.cn

[S07] C：数组遍历求和
来源：http://cue.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cub.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://gng.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jld.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://uoe.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gfp.ydjk.org.cn

[S10] C：指针与解引用
来源：http://uqq.zycfv.cn

int *p = &a;  *p = 5;
来源：http://moc.zdqjudy.top

[S11] C：逐行读文件
来源：http://pyv.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://qjx.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wyc.bbcook.cn

fclose(f);
来源：http://eev.jyoumei.cn

[S12] C：写文件
来源：http://vbr.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://msj.yj20258.top

[S13] C：宏定义
来源：http://mvf.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fpw.iojbl.cn

[S14] C：枚举
来源：http://hde.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://bcz.wangdashe.top

[S15] C：类型转换
来源：http://cif.quarkkingdee.top

(double) a / b
来源：http://izv.svipenyu.cn

[S16] C：位操作置位
来源：http://dhi.bbcook.cn

x |= (1 << 3);
来源：http://nzv.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://bsi.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://opd.iojbl.cn

[S18] C：命令行参数
来源：http://sov.xinyue.icu

int main(int argc, char **argv)
来源：http://mtp.gotoacloud.top

[S19] C：快速排序
来源：http://jtk.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://jfj.hnqzz.top

[S20] C：二分查找
来源：http://kkt.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bkp.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://uda.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jfy.epnwcf.com

[S22] C：字符串转数字
来源：http://gqt.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://eks.wangshuangyany.cn

[S23] C：随机数
来源：http://msb.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://noq.yonumen.top

[S24] C：获取本地时间
来源：http://flx.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zeb.fktsv.cn

[S25] C：内存拷贝
来源：http://fvg.guowangkeji.top

memcpy(dst, src, n);
来源：http://syq.wangshuangyany.cn

[S26] C：内存清零
来源：http://szx.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://cbz.xinyue.icu

[S27] C：定义常量
来源：http://spa.tian-w.cn

const double PI = 3.14159;
来源：http://kbe.xziqi.cn

[S28] C：静态变量
来源：http://itm.zhengqikj.top

static int counter = 0;
来源：http://vig.yfazqb.com

[S29] C：变参函数
来源：http://jgi.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eps.tarul.cn

[S30] C：头文件保护
来源：http://xac.jyoumei.cn

#ifndef X_H
来源：http://lvr.ywan-chungtsiang.top

#define X_H
来源：http://nlm.ctjpmb.com

#endif
来源：http://hil.yj20258888.top

[S31] C++：Hello World
来源：http://yeg.c1oappe.top

#include <iostream>
来源：http://elx.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://ueu.yangfankeji.com

[S32] C++：字符串
来源：http://lct.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://xvm.sysykeji.top

[S33] C++：vector 增删
来源：http://hfc.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nvo.sxryk.cn

[S34] C++：遍历 vector
来源：http://ykw.vqdsnc.cn

for (auto &x : v) { std::cout << x; }
来源：http://kie.dashuyun.cn

[S35] C++：map
来源：http://lha.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wqy.haohaochexian.top

[S36] C++：unordered_map
来源：http://tef.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bsa.jinqigfzy.top

[S37] C++：set
来源：http://cuj.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://czx.feifeiyinyue.top

[S38] C++：排序
来源：http://ovc.meibo888.top

std::sort(v.begin(), v.end());
来源：http://ujl.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://ebo.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jkn.zycfv.cn

[S40] C++：查找元素
来源：http://jfc.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eac.andypj.xyz


<!-- 参考信息 -->