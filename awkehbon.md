代发 wailian999

[Q67] 设置隔离级别
来源：http://ygq.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kub.daria6918.cn

[Q68] 保存点
来源：http://ctn.gzhubu.top

SAVEPOINT sp1;
来源：http://fbe.zhengqikj.top

ROLLBACK TO sp1;
来源：http://uzm.hysaishi.cn

[Q69] 查看执行计划
来源：http://pbv.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kjm.redwolf501.top

[Q70] 更新统计信息
来源：http://xsc.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://vva.redwolf501.top

[Q71] 查看建表语句
来源：http://elm.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jwt.ydzc1.top

[Q72] 查看索引
来源：http://ppa.ivvv.top

SHOW INDEX FROM users;
来源：http://rgv.jinqigfzy.top

[Q73] 查看表状态
来源：http://mai.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hjh.wangdashe.top

[Q74] 强制使用索引
来源：http://fyl.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uwg.svipenyu.cn

[Q75] 日期格式化
来源：http://uwa.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://obj.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kvd.snrcjt.cn

[Q76] 按天统计
来源：http://pqu.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kmu.nwbrower.top

[Q77] 时间加减
来源：http://dpr.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ufc.chenjidiqi.icu

[Q78] 当前时间
来源：http://jfn.shanyushiyangtech.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rke.yj20258888.top

[Q79] 字符串拼接
来源：http://agk.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ijc.cqqwz.cn

[Q80] 字符串截取
来源：http://jhl.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://atk.zycfv.cn

[Q81] 字符串替换
来源：http://kbh.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ewl.gotoacloud.top

[Q82] 字符长度与字节长度
来源：http://stq.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rju.kuanghao11.cn

[Q83] 大小写转换
来源：http://ynh.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rit.chenlongwang.top

[Q84] 去除首尾空格
来源：http://bgk.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://hjj.gzhubu.top

[Q85] 数值取整
来源：http://tpe.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wby.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://voq.iojbl.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ppj.daxiang520.top

[Q87] JSON 字段做条件
来源：http://xkb.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://adh.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://llp.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ggr.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dvi.cashguo.top

[Q89] 判断表是否存在
来源：http://ief.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xmd.0kj1m.cn

[Q90] 生成序号列
来源：http://nzi.smart0.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ebi.jinyuanbaomall.cn

================================================================================
来源：http://jsx.hammf.cn

R. Bash 专题
来源：http://wno.yonumen.top

================================================================================
来源：http://rdf.chenzaomai.com

[R01] shebang 与严格模式
来源：http://pjp.guowangkeji.top

#!/usr/bin/env bash
来源：http://kld.andypj.xyz

set -euo pipefail
来源：http://njo.gzhubu.top

[R02] 变量赋值与使用
来源：http://gym.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://vuy.dianchejie.cn

[R03] 只读变量
来源：http://jnk.c1oappe.top

readonly PI=3.14
来源：http://fxx.jqgufenzy.top

[R04] 位置参数
来源：http://hwh.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cck.tanke756.top

[R05] 参数默认值
来源：http://bab.epnwcf.com

name="${1:-default}"
来源：http://rmn.yangfankeji.com

[R06] 判断命令是否存在
来源：http://qhg.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pur.wangshuangyany.cn

[R07] if 判断文件
来源：http://cvd.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ced.tarul.cn

[R08] 数值比较
来源：http://hyj.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vrc.yanxiufei.cn

[R09] 字符串比较
来源：http://uau.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://suw.yangfankeji.com

[R10] 正则匹配
来源：http://kdh.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://twg.sufxvd.cn

[R11] case 多分支
来源：http://sxr.daria6918.cn

case "$1" in
来源：http://prg.smart0.xyz

start) echo "启动" ;;
来源：http://cij.bbcook.cn

stop)  echo "停止" ;;
来源：http://wrt.mhx1999.top

*)     echo "未知命令" ;;
来源：http://wds.pycfn.com

esac
来源：http://rac.vehdjk.com

[R12] for 遍历文件
来源：http://cnl.fanxiaobao.xyz

for f in *.txt; do echo "$f"; done
来源：http://wez.vehdjk.com

[R13] for 计数循环
来源：http://elr.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://ioq.hnqzz.top

[R14] C 风格 for
来源：http://mjf.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://emz.yonumen.top

[R15] while 逐行读文件
来源：http://lba.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yvp.dashuyun.cn

[R16] until 等待条件
来源：http://cvo.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lxx.pycfn.com

[R17] 数组定义与取值
来源：http://vce.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://qdz.svipenyu.cn

[R18] 遍历数组
来源：http://wic.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://far.zhoulong.xyz

[R19] 数组长度
来源：http://yaj.hysaishi.cn

echo "${#arr[@]}"
来源：http://tal.vehdjk.com

[R20] 关联数组（字典）
来源：http://afs.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zbd.pengpengdd.cyou

[R21] 字符串长度
来源：http://trj.316326.xyz

echo "${#s}"
来源：http://kbd.hnqzz.top

[R22] 截取子串
来源：http://spg.sjlbkw.cn

echo "${s:0:5}"
来源：http://nqa.jiagoushi.top

[R23] 字符串替换
来源：http://lgb.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xvb.zycfv.cn

[R24] 大小写转换
来源：http://gbh.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://bgw.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://sub.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://cdx.haohaochexian.top

[R26] 命令替换
来源：http://qls.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://eoy.yj20258.top

[R27] 算术展开
来源：http://tqy.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://hgp.gzhubu.top

[R28] 浮点运算
来源：http://hgg.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://bib.0kj1m.cn

[R29] 定义函数
来源：http://eyi.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hit.zhongyouzk.top

[R30] 函数返回状态码
来源：http://ykc.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://vuk.yuxming.cn

[R31] 局部变量
来源：http://mdj.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://rvi.sweek.top

[R32] 参数个数校验
来源：http://poi.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ayk.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://ove.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ozn.cashguo.top

[R34] 退出时清理
来源：http://jto.0kj1m.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vrx.yangfankeji.com

[R35] 后台执行并等待
来源：http://vqm.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uok.yongpay.top

[R36] 并发执行多个任务
来源：http://tut.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ocf.cashguo.top

[R37] 把输出赋给变量
来源：http://llp.birdmap.top

files=$(ls -1)
来源：http://ubc.bbcook.cn

[R38] 管道串联
来源：http://jal.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://kxo.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://jqz.yj202588.top

cmd > out.log 2>&1
来源：http://cus.hywenlv.cn

[R40] 追加写日志
来源：http://rgr.tianlin.xyz

echo "log" >> out.log
来源：http://sxj.hysaishi.cn

[R41] 丢弃输出
来源：http://ses.cheryme.top

cmd >/dev/null 2>&1
来源：http://fon.gaohongyu789.top

[R42] 输入重定向
来源：http://kku.epnwcf.com

wc -l < a.txt
来源：http://enf.xuanzx.com

[R43] 按名字查找文件
来源：http://zao.sjlbkw.cn

find . -name "*.log" -type f
来源：http://cfj.xinyue.icu

[R44] 按修改时间查找
来源：http://teb.yangfankeji.com

find . -mtime -7 -type f
来源：http://rqt.xingfuxueyuan.xyz

[R45] 批量删除
来源：http://tmr.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://sef.bbcook.cn

[R46] 递归替换文件内容
来源：http://pjf.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dor.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://plf.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://jgm.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://oqt.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://rlf.chenzaomai.com

[R49] awk 带条件
来源：http://ced.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oaw.meibo888.top

[R50] awk 求和
来源：http://pqy.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://rhw.xuanzx.com

[R51] 排序去重取前几
来源：http://elb.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qaf.guannengcc.top

[R52] 统计行数
来源：http://ukh.jinghuilouyu.cn

wc -l a.txt
来源：http://omj.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://hop.9152youxi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://muv.yfazqb.com

[R54] 比较两个文件
来源：http://gkh.smart0.xyz

diff a.txt b.txt
来源：http://asz.pengpengdd.cyou

[R55] 压缩与解压
来源：http://ivm.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://juz.hysaishi.cn

[R56] 远程拷贝
来源：http://ghf.hnxiangtu.top

scp file user@host:/path/
来源：http://nzt.yuanzhike.top

[R57] 远程执行命令
来源：http://axf.ydjk.org.cn

ssh user@host 'uptime'
来源：http://mnw.nanxuanxn.top

[R58] 下载文件
来源：http://jzz.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wmc.yj20258.top

[R59] 发 POST JSON
来源：http://klb.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xlw.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://sxp.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vcx.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://dke.feifeiyinyue.top

df -h;  du -sh *
来源：http://trn.shzxlz.cn

[R62] 找最占空间的文件
来源：http://itf.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://awe.smart0.xyz

[R63] 内存与进程
来源：http://wph.yj20258.top

free -h;  ps aux | grep nginx
来源：http://fbw.haohaochexian.top

[R64] 结束进程
来源：http://rdb.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://xnu.hysaishi.cn

[R65] 查看端口占用
来源：http://qcn.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pfz.xziqi.cn

[R66] 定时任务
来源：http://azn.shuidangran.top

crontab -e;  crontab -l
来源：http://arq.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://ufe.gogol.net.cn

openssl rand -hex 16
来源：http://ugb.hcnkem.com

[R68] 计算文件校验值
来源：http://mft.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://tfe.cdnleiting.top

[R69] 生成随机密码
来源：http://lvl.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://dsr.yonumen.top

[R70] 时间戳与互转
来源：http://bia.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://uum.dashuyun.cn

[R71] 日期格式化
来源：http://vfw.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mdi.yuanzhike.top

[R72] 等待端口就绪
来源：http://dab.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mcn.uphjek.com

[R73] 分割大日志
来源：http://tho.tarul.cn

split -l 1000 big.log part_
来源：http://xuv.xylfe.cn

[R74] 批量重命名
来源：http://pqz.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eat.meibo888.top

[R75] 导出环境变量
来源：http://iee.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://aid.ydzc1.top

[R76] 使用临时文件
来源：http://ilf.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mxg.xinyue.icu

[R77] 读取用户输入
来源：http://jah.daria6918.cn

read -rp "请输入: " ans
来源：http://hnx.iojbl.cn

[R78] 交互式菜单
来源：http://ewa.quarkkingdee.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zzl.yangfankeji.com

[R79] 解析命令行选项
来源：http://wmy.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fal.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://irp.pycfn.com

time ./run.sh
来源：http://dyh.yj20258.top

================================================================================
来源：http://idt.wangdashe.top

S. C / C++ 专题
来源：http://duy.birdmap.top

================================================================================
来源：http://scb.kuanghao11.cn

[S01] C：Hello World
来源：http://lbq.dianchejie.cn

#include <stdio.h>
来源：http://jtl.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://enh.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://ywq.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://asw.yuxming.cn

[S03] C：读入整数
来源：http://uyu.cqqwz.cn

int x; scanf("%d", &x);
来源：http://klk.dianchejie.cn

[S04] C：字符串复制
来源：http://wmj.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://oaq.pycfn.com

[S05] C：字符串长度
来源：http://cxp.jinghuilouyu.cn

strlen(s)
来源：http://vhm.jyoumei.cn

[S06] C：字符串比较
来源：http://dao.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://pdc.yj202588.top

[S07] C：数组遍历求和
来源：http://dnk.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pqn.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://see.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ehj.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://bxo.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hes.zycfv.cn

[S10] C：指针与解引用
来源：http://vxf.ydzc1.top

int *p = &a;  *p = 5;
来源：http://rpn.guannengcc.top

[S11] C：逐行读文件
来源：http://dud.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://dyp.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nce.sxryk.cn

fclose(f);
来源：http://dri.xuetiantiany.cn

[S12] C：写文件
来源：http://oxo.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ooj.0kj1m.cn

[S13] C：宏定义
来源：http://gvj.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sjo.chenlongwang.top

[S14] C：枚举
来源：http://gbv.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://usq.chenzaomai.com

[S15] C：类型转换
来源：http://koe.havefunace.top

(double) a / b
来源：http://eel.fengsongda.top

[S16] C：位操作置位
来源：http://hrh.sweek.top

x |= (1 << 3);
来源：http://xrd.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://nlf.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kjr.hcnkem.com

[S18] C：命令行参数
来源：http://wto.smart0.xyz

int main(int argc, char **argv)
来源：http://tjm.birdmap.top

[S19] C：快速排序
来源：http://agu.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://xak.yj202588.top

[S20] C：二分查找
来源：http://lim.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rgs.ydjk.org.cn

[S21] C：字符类别判断
来源：http://dxh.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lsn.daria6918.cn

[S22] C：字符串转数字
来源：http://ybg.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jvh.haohaochexian.top

[S23] C：随机数
来源：http://kzf.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eim.yuxming.cn

[S24] C：获取本地时间
来源：http://yff.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ubf.sufxvd.cn

[S25] C：内存拷贝
来源：http://vqx.bjfxy.top

memcpy(dst, src, n);
来源：http://erp.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://mvq.bbcook.cn

memset(a, 0, sizeof a);
来源：http://rfi.feifeiyinyue.top

[S27] C：定义常量
来源：http://lab.xuanzx.com

const double PI = 3.14159;
来源：http://qqx.fanxiaobao.xyz

[S28] C：静态变量
来源：http://ahw.ehwqpu.com

static int counter = 0;
来源：http://jwo.haohaochexian.top

[S29] C：变参函数
来源：http://qjx.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://chr.cqqwz.cn

[S30] C：头文件保护
来源：http://tjp.cheryme.top

#ifndef X_H
来源：http://hqg.zhengqikj.top

#define X_H
来源：http://hxq.tarul.cn

#endif
来源：http://gmq.pycfn.com

[S31] C++：Hello World
来源：http://wlb.vqdsnc.cn

#include <iostream>
来源：http://cdw.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://ozg.hfpthk.cn

[S32] C++：字符串
来源：http://oxo.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://rfr.gzhubu.top

[S33] C++：vector 增删
来源：http://qhq.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kvg.zdbjq.cn

[S34] C++：遍历 vector
来源：http://adc.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://ejr.ydzc1.top

[S35] C++：map
来源：http://vkl.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cct.dianchejie.cn

[S36] C++：unordered_map
来源：http://lkk.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zbx.hongshengwenyu.top


<!-- 参考信息 -->