代发 wailian999

ANALYZE TABLE users;
来源：http://cqu.nanxuanxn.top

[Q71] 查看建表语句
来源：http://tkm.iojbl.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hvi.zhengqikj.top

[Q72] 查看索引
来源：http://lso.ehwqpu.com

SHOW INDEX FROM users;
来源：http://kxq.xuanzx.com

[Q73] 查看表状态
来源：http://zyn.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://xds.52xcode.cn

[Q74] 强制使用索引
来源：http://adz.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pnn.c1oappe.top

[Q75] 日期格式化
来源：http://faa.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hwj.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wqy.gotoacloud.top

[Q76] 按天统计
来源：http://lfg.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://quu.shanyushiyangtech.top

[Q77] 时间加减
来源：http://mqn.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tgm.wangdashe.top

[Q78] 当前时间
来源：http://xek.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jqr.daria6918.cn

[Q79] 字符串拼接
来源：http://hdb.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://duw.gogol.net.cn

[Q80] 字符串截取
来源：http://jix.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zdm.sweek.top

[Q81] 字符串替换
来源：http://ijh.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rrz.cheryme.top

[Q82] 字符长度与字节长度
来源：http://cfx.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aad.ybcxt.top

[Q83] 大小写转换
来源：http://kdt.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bvl.hfpthk.cn

[Q84] 去除首尾空格
来源：http://qrw.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://vmr.tarul.cn

[Q85] 数值取整
来源：http://hda.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tus.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://luf.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jjv.sweek.top

[Q87] JSON 字段做条件
来源：http://sdt.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ljs.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://kkh.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://znx.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oev.yuanzhike.top

[Q89] 判断表是否存在
来源：http://fbr.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cvx.tianlin.xyz

[Q90] 生成序号列
来源：http://vdx.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qdr.sjlbkw.cn

================================================================================
来源：http://nuo.9152youxi.cn

R. Bash 专题
来源：http://duv.wangshuangyany.cn

================================================================================
来源：http://nzi.yueranfly.top

[R01] shebang 与严格模式
来源：http://hwz.jlsjyb.cn

#!/usr/bin/env bash
来源：http://ash.jianghu66.top

set -euo pipefail
来源：http://pht.9152youxi.cn

[R02] 变量赋值与使用
来源：http://jhy.xuanzx.com

name="Tom"; echo "$name"
来源：http://fxe.xylfe.cn

[R03] 只读变量
来源：http://qqi.jiagoushi.top

readonly PI=3.14
来源：http://zat.xziqi.cn

[R04] 位置参数
来源：http://jth.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qxw.chenzaomai.com

[R05] 参数默认值
来源：http://ckb.nwbrower.top

name="${1:-default}"
来源：http://sjx.bjfxy.top

[R06] 判断命令是否存在
来源：http://otj.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pxy.yj202588.top

[R07] if 判断文件
来源：http://pmy.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://duy.jiagoushi.top

[R08] 数值比较
来源：http://gsn.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iwy.zhiwuduotai.top

[R09] 字符串比较
来源：http://lud.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ycc.cucudq.cn

[R10] 正则匹配
来源：http://xoq.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nkl.hywenlv.cn

[R11] case 多分支
来源：http://wrq.shuidangran.top

case "$1" in
来源：http://ckq.cashguo.top

start) echo "启动" ;;
来源：http://bff.ivvv.top

stop)  echo "停止" ;;
来源：http://ise.sweek.top

*)     echo "未知命令" ;;
来源：http://xbe.zhongyouzk.top

esac
来源：http://pau.9152youxi.cn

[R12] for 遍历文件
来源：http://weu.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://oxt.fengsongda.top

[R13] for 计数循环
来源：http://glc.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ygb.bjfxy.top

[R14] C 风格 for
来源：http://opq.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rkx.9152youxi.cn

[R15] while 逐行读文件
来源：http://ags.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dds.zhijiandao.cn

[R16] until 等待条件
来源：http://dxy.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://anm.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://bgb.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lnc.yj20258888.top

[R18] 遍历数组
来源：http://lyj.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vzk.yj20258.top

[R19] 数组长度
来源：http://mwl.sufxvd.cn

echo "${#arr[@]}"
来源：http://qsb.hesvh.cn

[R20] 关联数组（字典）
来源：http://pzh.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dpm.zdqjudy.top

[R21] 字符串长度
来源：http://vjt.gogol.net.cn

echo "${#s}"
来源：http://yow.zhaomingkeji.xyz

[R22] 截取子串
来源：http://uhn.yj202588.top

echo "${s:0:5}"
来源：http://wfw.iojbl.cn

[R23] 字符串替换
来源：http://sbf.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://emj.zdbjq.cn

[R24] 大小写转换
来源：http://jna.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://dvz.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://jmh.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://frg.sjlbkw.cn

[R26] 命令替换
来源：http://lbq.cheryme.top

now=$(date +%F); echo "$now"
来源：http://pfp.aibaodan.cn

[R27] 算术展开
来源：http://fuf.yuxming.cn

echo $((1 + 2 * 3))
来源：http://wdl.yueranfly.top

[R28] 浮点运算
来源：http://rqs.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://cga.sjlbkw.cn

[R29] 定义函数
来源：http://zar.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://apk.yj20258888.top

[R30] 函数返回状态码
来源：http://gcz.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://vnv.52xcode.cn

[R31] 局部变量
来源：http://upu.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://kjs.nwbrower.top

[R32] 参数个数校验
来源：http://xcd.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vrm.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://jha.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ruz.cqqwz.cn

[R34] 退出时清理
来源：http://ehh.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://jni.sxryk.cn

[R35] 后台执行并等待
来源：http://nko.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://oqa.fehbvm.com

[R36] 并发执行多个任务
来源：http://zoc.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zku.chenlongwang.top

[R37] 把输出赋给变量
来源：http://mpy.fktsv.cn

files=$(ls -1)
来源：http://svz.cucudq.cn

[R38] 管道串联
来源：http://vrd.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://utv.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://jve.yueranfly.top

cmd > out.log 2>&1
来源：http://ljl.wangshuangyany.cn

[R40] 追加写日志
来源：http://ocz.epnwcf.com

echo "log" >> out.log
来源：http://izc.yj20258.top

[R41] 丢弃输出
来源：http://ifi.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://fre.sxryk.cn

[R42] 输入重定向
来源：http://npl.fktsv.cn

wc -l < a.txt
来源：http://sju.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://tml.hcnkem.com

find . -name "*.log" -type f
来源：http://alx.ehwqpu.com

[R44] 按修改时间查找
来源：http://cqt.yuxming.cn

find . -mtime -7 -type f
来源：http://gxm.ydzc1.top

[R45] 批量删除
来源：http://efp.cheryme.top

find . -name "*.tmp" -delete
来源：http://hxg.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://ief.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wcj.9152youxi.cn

[R47] sed 单行替换
来源：http://zfk.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://qav.jqgufenzy.top

[R48] awk 取指定列
来源：http://wem.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://oso.tarul.cn

[R49] awk 带条件
来源：http://msp.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://syu.zhengqikj.top

[R50] awk 求和
来源：http://qmh.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://wuo.sxryk.cn

[R51] 排序去重取前几
来源：http://gsd.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://xzi.zdqjudy.top

[R52] 统计行数
来源：http://ebn.pengpengdd.cyou

wc -l a.txt
来源：http://gjm.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://wpn.cucudq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ehx.9152youxi.cn

[R54] 比较两个文件
来源：http://iin.zhixingplan.top

diff a.txt b.txt
来源：http://wdn.jqgufenzy.top

[R55] 压缩与解压
来源：http://unp.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iol.jqgufenzy.top

[R56] 远程拷贝
来源：http://zte.andypj.xyz

scp file user@host:/path/
来源：http://hmc.mhx1999.top

[R57] 远程执行命令
来源：http://xey.mhx1999.top

ssh user@host 'uptime'
来源：http://ciq.jinyuanbaomall.cn

[R58] 下载文件
来源：http://gcr.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://azp.gaohongyu789.top

[R59] 发 POST JSON
来源：http://suv.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yso.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://cpq.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zbu.guowangkeji.top

[R61] 磁盘占用
来源：http://bcb.sysykeji.top

df -h;  du -sh *
来源：http://fuz.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://ssz.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://yzm.fanxiaobao.xyz

[R63] 内存与进程
来源：http://rou.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://ogn.cashguo.top

[R64] 结束进程
来源：http://oga.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://czq.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://lgr.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hjw.yj20258888.top

[R66] 定时任务
来源：http://ast.jiagoushi.top

crontab -e;  crontab -l
来源：http://wvy.bjfxy.top

[R67] 生成随机十六进制串
来源：http://boo.ybcxt.top

openssl rand -hex 16
来源：http://shu.haohaochexian.top

[R68] 计算文件校验值
来源：http://orz.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://pba.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://hyo.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://wbh.jqgfzy.top

[R70] 时间戳与互转
来源：http://ghy.cheryme.top

date +%s;  date -d @1700000000
来源：http://ptx.feifeiyinyue.top

[R71] 日期格式化
来源：http://otz.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nhg.hesvh.cn

[R72] 等待端口就绪
来源：http://ozr.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mpx.hcnkem.com

[R73] 分割大日志
来源：http://xyg.guowangkeji.top

split -l 1000 big.log part_
来源：http://gjf.gaohongyu789.top

[R74] 批量重命名
来源：http://acd.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ttm.havefunace.top

[R75] 导出环境变量
来源：http://xfq.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://yuh.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://ivn.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ykr.fehbvm.com

[R77] 读取用户输入
来源：http://vfb.zhoulong.xyz

read -rp "请输入: " ans
来源：http://wex.meibo888.top

[R78] 交互式菜单
来源：http://yii.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://hpm.hnqzz.top

[R79] 解析命令行选项
来源：http://nin.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://car.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://cme.fzhhl.top

time ./run.sh
来源：http://xgm.xuetiantiany.cn

================================================================================
来源：http://rum.daria6918.cn

S. C / C++ 专题
来源：http://lcu.shanyushiyangtech.top

================================================================================
来源：http://max.dashuyun.cn

[S01] C：Hello World
来源：http://yqd.smart0.xyz

#include <stdio.h>
来源：http://rmx.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lmf.tanke756.top

[S02] C：变量与格式化输出
来源：http://ame.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://iys.aizwys.cn

[S03] C：读入整数
来源：http://fgm.chenlongwang.top

int x; scanf("%d", &x);
来源：http://yej.hywenlv.cn

[S04] C：字符串复制
来源：http://xug.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hbm.ydjk.org.cn

[S05] C：字符串长度
来源：http://fap.daxiang520.top

strlen(s)
来源：http://jtx.tian-w.cn

[S06] C：字符串比较
来源：http://xpn.zycfv.cn

strcmp(a, b) == 0
来源：http://yll.ivvv.top

[S07] C：数组遍历求和
来源：http://nnm.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nbk.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://hij.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lyk.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://jeo.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wiv.52xcode.cn

[S10] C：指针与解引用
来源：http://fse.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://jnu.sweek.top

[S11] C：逐行读文件
来源：http://uff.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://ayd.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zuu.hcnkem.com

fclose(f);
来源：http://zwd.birdmap.top

[S12] C：写文件
来源：http://ome.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gtx.ivvv.top

[S13] C：宏定义
来源：http://ory.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yqz.zhongyouzk.top

[S14] C：枚举
来源：http://rvf.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://uld.gzhubu.top

[S15] C：类型转换
来源：http://zsl.yongpay.top

(double) a / b
来源：http://zap.tarul.cn

[S16] C：位操作置位
来源：http://ifw.yj20258.top

x |= (1 << 3);
来源：http://huc.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://quy.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gac.uphjek.com

[S18] C：命令行参数
来源：http://ahv.hywenlv.cn

int main(int argc, char **argv)
来源：http://opj.fehbvm.com

[S19] C：快速排序
来源：http://niw.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zel.vqdsnc.cn

[S20] C：二分查找
来源：http://olf.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xag.bjfxy.top

[S21] C：字符类别判断
来源：http://mmt.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pej.haohaochexian.top

[S22] C：字符串转数字
来源：http://xss.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uay.xuanzx.com

[S23] C：随机数
来源：http://ldi.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kra.iojbl.cn

[S24] C：获取本地时间
来源：http://hgk.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rim.tarul.cn

[S25] C：内存拷贝
来源：http://nfj.hcnkem.com

memcpy(dst, src, n);
来源：http://wuc.ydjk.org.cn

[S26] C：内存清零
来源：http://wys.316326.xyz

memset(a, 0, sizeof a);
来源：http://gmw.xuetiantiany.cn

[S27] C：定义常量
来源：http://spk.shzxlz.cn

const double PI = 3.14159;
来源：http://spz.meibo888.top

[S28] C：静态变量
来源：http://hyq.uphjek.com

static int counter = 0;
来源：http://kgz.aibaodan.cn

[S29] C：变参函数
来源：http://ert.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hlh.redwolf501.top

[S30] C：头文件保护
来源：http://jue.xuetiantiany.cn

#ifndef X_H
来源：http://ahg.epnwcf.com

#define X_H
来源：http://ppo.sweek.top

#endif
来源：http://ugo.52xcode.cn

[S31] C++：Hello World
来源：http://uxk.0kj1m.cn

#include <iostream>
来源：http://bsr.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://iet.zhongyouzk.top

[S32] C++：字符串
来源：http://ddh.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://lej.c1oappe.top

[S33] C++：vector 增删
来源：http://xzp.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kbx.guannengcc.top

[S34] C++：遍历 vector
来源：http://dbn.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://tgw.hysaishi.cn

[S35] C++：map
来源：http://vep.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hta.kuanghao11.cn

[S36] C++：unordered_map
来源：http://jkm.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pjh.fzhhl.top

[S37] C++：set
来源：http://ale.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bxz.jyoumei.cn

[S38] C++：排序
来源：http://qzu.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://fsy.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://xwp.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hle.ybcxt.top

[S40] C++：查找元素
来源：http://uwn.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mfk.sxryk.cn


<!-- 参考信息 -->