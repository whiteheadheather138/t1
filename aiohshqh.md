代发 wailian999

[Q65] 回滚事务
来源：http://muu.c1oappe.top

ROLLBACK;
来源：http://usq.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://hee.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vic.aibaodan.cn

[Q67] 设置隔离级别
来源：http://wec.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zud.nwbrower.top

[Q68] 保存点
来源：http://wav.yj202588.top

SAVEPOINT sp1;
来源：http://leb.nwbrower.top

ROLLBACK TO sp1;
来源：http://ltp.ivvv.top

[Q69] 查看执行计划
来源：http://hsq.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hzp.pengpengdd.cyou

[Q70] 更新统计信息
来源：http://fan.xziqi.cn

ANALYZE TABLE users;
来源：http://znn.smart0.xyz

[Q71] 查看建表语句
来源：http://sfw.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://llu.tianlin.xyz

[Q72] 查看索引
来源：http://gac.daria6918.cn

SHOW INDEX FROM users;
来源：http://ous.xuanzx.com

[Q73] 查看表状态
来源：http://ehi.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mgz.jinqigufen.top

[Q74] 强制使用索引
来源：http://wkv.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fqr.redwolf501.top

[Q75] 日期格式化
来源：http://fgo.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yeo.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zgj.xuetiantiany.cn

[Q76] 按天统计
来源：http://vgx.hywenlv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iec.yj20258888.top

[Q77] 时间加减
来源：http://uqg.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oby.xuanzx.com

[Q78] 当前时间
来源：http://sgm.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ggz.52xcode.cn

[Q79] 字符串拼接
来源：http://rja.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ssw.jiagoushi.top

[Q80] 字符串截取
来源：http://lqi.yuxming.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wyy.cashguo.top

[Q81] 字符串替换
来源：http://red.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sha.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://wnt.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xmk.yj20258.top

[Q83] 大小写转换
来源：http://ojo.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pgk.yueranfly.top

[Q84] 去除首尾空格
来源：http://lck.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://pnw.tarul.cn

[Q85] 数值取整
来源：http://axn.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://plp.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://uze.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tfr.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://wsx.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://psx.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://amo.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dvm.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kmf.hysaishi.cn

[Q89] 判断表是否存在
来源：http://wqq.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lrf.ctjpmb.com

[Q90] 生成序号列
来源：http://ccx.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hjz.daria6918.cn

================================================================================
来源：http://huz.sweek.top

R. Bash 专题
来源：http://rvv.fehbvm.com

================================================================================
来源：http://yfz.sxryk.cn

[R01] shebang 与严格模式
来源：http://rvo.dashuyun.cn

#!/usr/bin/env bash
来源：http://duh.meibo888.top

set -euo pipefail
来源：http://qrt.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://wgh.aizwys.cn

name="Tom"; echo "$name"
来源：http://uyg.cqqwz.cn

[R03] 只读变量
来源：http://bnm.jinqigufen.top

readonly PI=3.14
来源：http://zlf.cashguo.top

[R04] 位置参数
来源：http://ocb.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uwf.316326.xyz

[R05] 参数默认值
来源：http://lsx.nanxuanxn.top

name="${1:-default}"
来源：http://vjs.jqgfzy.top

[R06] 判断命令是否存在
来源：http://ozs.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fxd.uphjek.com

[R07] if 判断文件
来源：http://cvt.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cbp.redwolf501.top

[R08] 数值比较
来源：http://fma.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://plq.zhiwuduotai.top

[R09] 字符串比较
来源：http://mwi.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://toe.yfazqb.com

[R10] 正则匹配
来源：http://mzs.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sar.cdnleiting.top

[R11] case 多分支
来源：http://ejl.epnwcf.com

case "$1" in
来源：http://wwp.ctjpmb.com

start) echo "启动" ;;
来源：http://mwg.ivvv.top

stop)  echo "停止" ;;
来源：http://fuy.hammf.cn

*)     echo "未知命令" ;;
来源：http://kfr.gotoacloud.top

esac
来源：http://mjy.zhongyouzk.top

[R12] for 遍历文件
来源：http://gmi.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://leg.yanxiufei.cn

[R13] for 计数循环
来源：http://peq.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://tru.quarkkingdee.top

[R14] C 风格 for
来源：http://gve.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lvc.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://sxp.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://izs.wangdashe.top

[R16] until 等待条件
来源：http://dad.tian-w.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://svy.daria6918.cn

[R17] 数组定义与取值
来源：http://hvd.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://uoo.kuanghao11.cn

[R18] 遍历数组
来源：http://xsb.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uwv.tian-w.cn

[R19] 数组长度
来源：http://kpf.dianchejie.cn

echo "${#arr[@]}"
来源：http://adm.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://hhm.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yks.pengpengdd.cyou

[R21] 字符串长度
来源：http://hsl.fanxiaobao.xyz

echo "${#s}"
来源：http://htg.nanxuanxn.top

[R22] 截取子串
来源：http://mct.redwolf501.top

echo "${s:0:5}"
来源：http://yzt.fengsongda.top

[R23] 字符串替换
来源：http://cnt.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://met.fktsv.cn

[R24] 大小写转换
来源：http://oiu.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ryy.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://kfy.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wbe.fengsongda.top

[R26] 命令替换
来源：http://cnp.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://qcf.ppjwa.cn

[R27] 算术展开
来源：http://nfj.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://npo.nwbrower.top

[R28] 浮点运算
来源：http://zqq.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://kte.hongshengwenyu.top

[R29] 定义函数
来源：http://skg.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ypr.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://iro.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://qcu.zhoulong.xyz

[R31] 局部变量
来源：http://skr.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://lvj.yuxming.cn

[R32] 参数个数校验
来源：http://vwl.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dnh.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://plj.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ieh.cheryme.top

[R34] 退出时清理
来源：http://dnr.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://kkw.yj20258888.top

[R35] 后台执行并等待
来源：http://ypq.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zdg.xziqi.cn

[R36] 并发执行多个任务
来源：http://jex.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tbg.hammf.cn

[R37] 把输出赋给变量
来源：http://ikn.yfazqb.com

files=$(ls -1)
来源：http://viz.daxiang520.top

[R38] 管道串联
来源：http://pmy.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://byx.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://iro.redwolf501.top

cmd > out.log 2>&1
来源：http://bwi.hysaishi.cn

[R40] 追加写日志
来源：http://nqd.dianchejie.cn

echo "log" >> out.log
来源：http://spt.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://ehf.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://caa.fehbvm.com

[R42] 输入重定向
来源：http://roc.nanxuanxn.top

wc -l < a.txt
来源：http://xzy.hywenlv.cn

[R43] 按名字查找文件
来源：http://sgv.nanxuanxn.top

find . -name "*.log" -type f
来源：http://yjf.svipenyu.cn

[R44] 按修改时间查找
来源：http://ydt.sxryk.cn

find . -mtime -7 -type f
来源：http://bbw.tarul.cn

[R45] 批量删除
来源：http://vkd.tanke756.top

find . -name "*.tmp" -delete
来源：http://mmi.sufxvd.cn

[R46] 递归替换文件内容
来源：http://gkx.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zpy.jqgufenzy.top

[R47] sed 单行替换
来源：http://fgm.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://dfe.jianghu66.top

[R48] awk 取指定列
来源：http://wqi.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://prb.sweek.top

[R49] awk 带条件
来源：http://evf.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wpr.yj20258888.top

[R50] awk 求和
来源：http://gib.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vzu.haohaochexian.top

[R51] 排序去重取前几
来源：http://jxb.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://orb.xuetiantiany.cn

[R52] 统计行数
来源：http://tcq.jqgufenzy.top

wc -l a.txt
来源：http://qja.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://fby.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pus.316326.xyz

[R54] 比较两个文件
来源：http://ivy.jianghu66.top

diff a.txt b.txt
来源：http://ejj.sxryk.cn

[R55] 压缩与解压
来源：http://zwt.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ocs.wangdashe.top

[R56] 远程拷贝
来源：http://bej.dashuyun.cn

scp file user@host:/path/
来源：http://eju.zhoulong.xyz

[R57] 远程执行命令
来源：http://rkm.52xcode.cn

ssh user@host 'uptime'
来源：http://gzl.chenlongwang.top

[R58] 下载文件
来源：http://oqj.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tfy.redwolf501.top

[R59] 发 POST JSON
来源：http://evm.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://khs.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://fxi.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tpy.daria6918.cn

[R61] 磁盘占用
来源：http://flt.316326.xyz

df -h;  du -sh *
来源：http://vto.yvedp.cn

[R62] 找最占空间的文件
来源：http://bxn.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://wic.fzhhl.top

[R63] 内存与进程
来源：http://gqm.yj202588.top

free -h;  ps aux | grep nginx
来源：http://mys.wangshuangyany.cn

[R64] 结束进程
来源：http://kca.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://exx.hysaishi.cn

[R65] 查看端口占用
来源：http://dbu.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zev.9152youxi.cn

[R66] 定时任务
来源：http://ito.hnqzz.top

crontab -e;  crontab -l
来源：http://jxt.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://bwc.tian-w.cn

openssl rand -hex 16
来源：http://iem.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://yjh.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://huv.pycfn.com

[R69] 生成随机密码
来源：http://juw.chenlongwang.top

head -c 16 /dev/urandom | base64
来源：http://pqu.zhixingplan.top

[R70] 时间戳与互转
来源：http://ohz.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://tio.ydjk.org.cn

[R71] 日期格式化
来源：http://gba.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kyr.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://srg.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://dam.ivvv.top

[R73] 分割大日志
来源：http://avg.xuanzx.com

split -l 1000 big.log part_
来源：http://gnz.yj20258888.top

[R74] 批量重命名
来源：http://bjw.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gdx.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://auc.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://dax.yj202588.top

[R76] 使用临时文件
来源：http://jlp.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jfe.smart0.xyz

[R77] 读取用户输入
来源：http://oxb.sweek.top

read -rp "请输入: " ans
来源：http://wsj.sjlbkw.cn

[R78] 交互式菜单
来源：http://ltz.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://jvb.ydzc1.top

[R79] 解析命令行选项
来源：http://myi.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dqo.snrcjt.cn

[R80] 查看脚本执行耗时
来源：http://aty.ydjk.org.cn

time ./run.sh
来源：http://axm.wangdashe.top

================================================================================
来源：http://mgi.xylfe.cn

S. C / C++ 专题
来源：http://mdf.fehbvm.com

================================================================================
来源：http://det.jinqigufen.top

[S01] C：Hello World
来源：http://xkc.ehwqpu.com

#include <stdio.h>
来源：http://xty.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zgb.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://arw.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://kgo.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://fto.yuxming.cn

int x; scanf("%d", &x);
来源：http://btq.jqgufenzy.top

[S04] C：字符串复制
来源：http://hqu.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://qqi.hysaishi.cn

[S05] C：字符串长度
来源：http://erb.gotoacloud.top

strlen(s)
来源：http://bir.bbcook.cn

[S06] C：字符串比较
来源：http://otv.dianchejie.cn

strcmp(a, b) == 0
来源：http://pqw.cheryme.top

[S07] C：数组遍历求和
来源：http://bbo.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zcp.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://oce.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zwz.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://pje.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dur.hfpthk.cn

[S10] C：指针与解引用
来源：http://zny.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://xvz.hnxiangtu.top

[S11] C：逐行读文件
来源：http://jcf.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://mga.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vas.hnqzz.top

fclose(f);
来源：http://njr.zhaomingkeji.xyz

[S12] C：写文件
来源：http://bav.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gzp.tanke756.top

[S13] C：宏定义
来源：http://xsj.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://odm.hnqzz.top

[S14] C：枚举
来源：http://vwq.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://fvu.yueranfly.top

[S15] C：类型转换
来源：http://oic.hnxiangtu.top

(double) a / b
来源：http://bgc.0kj1m.cn

[S16] C：位操作置位
来源：http://eaw.yj20258.top

x |= (1 << 3);
来源：http://uxj.xziqi.cn

[S17] C：安全拼接字符串
来源：http://wwf.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://agy.zdqjudy.top

[S18] C：命令行参数
来源：http://mve.nwbrower.top

int main(int argc, char **argv)
来源：http://gzh.yangfankeji.com

[S19] C：快速排序
来源：http://nsb.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://pvq.daxiang520.top

[S20] C：二分查找
来源：http://mwu.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vpl.nanxuanxn.top

[S21] C：字符类别判断
来源：http://rwi.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nbu.guowangkeji.top

[S22] C：字符串转数字
来源：http://sdw.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fmp.cqqwz.cn

[S23] C：随机数
来源：http://vsn.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xlx.0kj1m.cn

[S24] C：获取本地时间
来源：http://ocl.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bbs.chenlongwang.top

[S25] C：内存拷贝
来源：http://xdb.xuanzx.com

memcpy(dst, src, n);
来源：http://htf.yueranfly.top

[S26] C：内存清零
来源：http://rlm.hcnkem.com

memset(a, 0, sizeof a);
来源：http://ifu.tanke756.top

[S27] C：定义常量
来源：http://odj.guowangkeji.top

const double PI = 3.14159;
来源：http://lnp.shanyushiyangtech.top

[S28] C：静态变量
来源：http://ncz.jinghuilouyu.cn

static int counter = 0;
来源：http://vqt.guowangkeji.top

[S29] C：变参函数
来源：http://voq.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qhs.yonumen.top

[S30] C：头文件保护
来源：http://yti.shanyushiyangkeji.top

#ifndef X_H
来源：http://dam.zhengqikj.top

#define X_H
来源：http://kil.hnqzz.top

#endif
来源：http://gyl.fzhhl.top

[S31] C++：Hello World
来源：http://nau.hongshengwenyu.top

#include <iostream>
来源：http://ufs.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://tvj.smart0.xyz

[S32] C++：字符串
来源：http://kht.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://fio.gotoacloud.top

[S33] C++：vector 增删
来源：http://sht.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mep.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://teu.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://sgp.zycfv.cn


<!-- 参考信息 -->