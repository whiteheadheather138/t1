代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://txk.sweek.top

[Q58] 累计求和
来源：http://ugk.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iag.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://uvu.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://svu.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://ulf.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ree.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zhb.kuanghao11.cn

[Q61] 移动平均
来源：http://rrl.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cvz.cdnleiting.top

[Q62] 分组占比
来源：http://cnn.yueranfly.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sdl.xinyue.icu

[Q63] 开启事务
来源：http://urj.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fmr.zycfv.cn

[Q64] 提交事务
来源：http://rsi.cdnleiting.top

COMMIT;
来源：http://eps.hongshengwenyu.top

[Q65] 回滚事务
来源：http://jgf.jinqigfzy.top

ROLLBACK;
来源：http://eul.hesvh.cn

[Q66] 行锁查询
来源：http://kpl.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://psz.yj20258.top

[Q67] 设置隔离级别
来源：http://ysn.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zel.zhongyouzk.top

[Q68] 保存点
来源：http://xqt.ydzc1.top

SAVEPOINT sp1;
来源：http://evu.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://wez.fzhhl.top

[Q69] 查看执行计划
来源：http://rts.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://feo.zdqjudy.top

[Q70] 更新统计信息
来源：http://fzq.gzhubu.top

ANALYZE TABLE users;
来源：http://njm.jqgufenzy.top

[Q71] 查看建表语句
来源：http://wwc.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://opz.dianchejie.cn

[Q72] 查看索引
来源：http://esz.jianghu66.top

SHOW INDEX FROM users;
来源：http://mzm.kuanghao11.cn

[Q73] 查看表状态
来源：http://ths.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vwz.ydzc1.top

[Q74] 强制使用索引
来源：http://xwh.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ilf.dianchejie.cn

[Q75] 日期格式化
来源：http://kee.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eja.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dhq.jyoumei.cn

[Q76] 按天统计
来源：http://xmm.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cwq.haohaochexian.top

[Q77] 时间加减
来源：http://iya.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tng.quarkkingdee.top

[Q78] 当前时间
来源：http://yvs.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://szl.zhijiandao.cn

[Q79] 字符串拼接
来源：http://wkr.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ggq.xuetiantiany.cn

[Q80] 字符串截取
来源：http://lxi.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kdu.ydjk.org.cn

[Q81] 字符串替换
来源：http://xko.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ibi.dianchejie.cn

[Q82] 字符长度与字节长度
来源：http://yye.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hix.jinqigufen.top

[Q83] 大小写转换
来源：http://gcl.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kek.svipenyu.cn

[Q84] 去除首尾空格
来源：http://nth.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://snd.chenjidiqi.icu

[Q85] 数值取整
来源：http://kuo.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dak.yj20258.top

[Q86] 读取 JSON 字段
来源：http://ibf.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lyz.ybcxt.top

[Q87] JSON 字段做条件
来源：http://sqw.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lrc.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://bjy.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cxv.52xcode.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kvc.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://pfn.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://atj.nwbrower.top

[Q90] 生成序号列
来源：http://auq.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lwi.xuetiantiany.cn

================================================================================
来源：http://reb.hongshengwenyu.top

R. Bash 专题
来源：http://xha.nanxinkj.top

================================================================================
来源：http://sqy.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://xpq.yuxming.cn

#!/usr/bin/env bash
来源：http://nje.316326.xyz

set -euo pipefail
来源：http://thk.fktsv.cn

[R02] 变量赋值与使用
来源：http://uzh.jinqigufen.top

name="Tom"; echo "$name"
来源：http://ioh.chenzaomai.com

[R03] 只读变量
来源：http://ady.hysaishi.cn

readonly PI=3.14
来源：http://dqs.kuanghao11.cn

[R04] 位置参数
来源：http://lvx.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rni.chenzaomai.com

[R05] 参数默认值
来源：http://dhj.zdbjq.cn

name="${1:-default}"
来源：http://srb.jqgfzy.top

[R06] 判断命令是否存在
来源：http://zov.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rat.zhengqikj.top

[R07] if 判断文件
来源：http://ogf.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vdb.jqgfzy.top

[R08] 数值比较
来源：http://nke.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://twr.jianghu66.top

[R09] 字符串比较
来源：http://sct.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mfe.yonumen.top

[R10] 正则匹配
来源：http://hmc.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mws.9152youxi.cn

[R11] case 多分支
来源：http://xnm.ywan-chungtsiang.top

case "$1" in
来源：http://plx.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://tok.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://bxc.aizwys.cn

*)     echo "未知命令" ;;
来源：http://tnq.jianghu66.top

esac
来源：http://eio.shangyingyoupin.top

[R12] for 遍历文件
来源：http://hii.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://tqj.ydjk.org.cn

[R13] for 计数循环
来源：http://jbr.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://dcf.cheryme.top

[R14] C 风格 for
来源：http://eha.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tio.iojbl.cn

[R15] while 逐行读文件
来源：http://hub.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xyr.wangshuangyany.cn

[R16] until 等待条件
来源：http://tkp.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qzv.redwolf501.top

[R17] 数组定义与取值
来源：http://xkz.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rob.vqdsnc.cn

[R18] 遍历数组
来源：http://tpl.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xzw.fehbvm.com

[R19] 数组长度
来源：http://yxx.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://ial.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://qpr.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zsw.sufxvd.cn

[R21] 字符串长度
来源：http://zei.ctjpmb.com

echo "${#s}"
来源：http://xal.0kj1m.cn

[R22] 截取子串
来源：http://hth.dashuyun.cn

echo "${s:0:5}"
来源：http://dbd.ydjk.org.cn

[R23] 字符串替换
来源：http://ehb.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rpu.bjfxy.top

[R24] 大小写转换
来源：http://ika.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://paj.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://ofu.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://alb.gotoacloud.top

[R26] 命令替换
来源：http://sgd.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://css.jinqigufen.top

[R27] 算术展开
来源：http://txs.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://hmo.hesvh.cn

[R28] 浮点运算
来源：http://ozt.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://brv.iojbl.cn

[R29] 定义函数
来源：http://uwi.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://siw.meibo888.top

[R30] 函数返回状态码
来源：http://wqq.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://wkt.zhijiandao.cn

[R31] 局部变量
来源：http://hbc.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://whk.hysaishi.cn

[R32] 参数个数校验
来源：http://xjo.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pbl.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://xwf.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yac.xylfe.cn

[R34] 退出时清理
来源：http://pwl.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://yhg.jiagoushi.top

[R35] 后台执行并等待
来源：http://nlg.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rab.zhixingplan.top

[R36] 并发执行多个任务
来源：http://rhg.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jix.sufxvd.cn

[R37] 把输出赋给变量
来源：http://rds.xinyue.icu

files=$(ls -1)
来源：http://svm.c1oappe.top

[R38] 管道串联
来源：http://ukd.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://dgq.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://byh.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://lxu.gogol.net.cn

[R40] 追加写日志
来源：http://sgm.pengpengdd.cyou

echo "log" >> out.log
来源：http://igt.hnqzz.top

[R41] 丢弃输出
来源：http://crq.shuidangran.top

cmd >/dev/null 2>&1
来源：http://hau.jyoumei.cn

[R42] 输入重定向
来源：http://awa.xinyue.icu

wc -l < a.txt
来源：http://nye.chenzaomai.com

[R43] 按名字查找文件
来源：http://mdr.zhongyouzk.top

find . -name "*.log" -type f
来源：http://gil.ehwqpu.com

[R44] 按修改时间查找
来源：http://dlo.tarul.cn

find . -mtime -7 -type f
来源：http://jab.zhaomingkeji.xyz

[R45] 批量删除
来源：http://urf.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://btv.sweek.top

[R46] 递归替换文件内容
来源：http://wxw.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mup.chenzaomai.com

[R47] sed 单行替换
来源：http://vbi.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://zpx.gaohongyu789.top

[R48] awk 取指定列
来源：http://wmv.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://mbp.hesvh.cn

[R49] awk 带条件
来源：http://kux.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jmt.redwolf501.top

[R50] awk 求和
来源：http://hzz.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wdy.gotoacloud.top

[R51] 排序去重取前几
来源：http://dmu.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qeq.guannengcc.top

[R52] 统计行数
来源：http://ujn.jianghu66.top

wc -l a.txt
来源：http://owl.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://gph.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xzb.hammf.cn

[R54] 比较两个文件
来源：http://lnv.hnqzz.top

diff a.txt b.txt
来源：http://vyi.haohaochexian.top

[R55] 压缩与解压
来源：http://lxr.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mbv.chenzaomai.com

[R56] 远程拷贝
来源：http://brc.gaohongyu789.top

scp file user@host:/path/
来源：http://pjg.bjfxy.top

[R57] 远程执行命令
来源：http://kfl.ybcxt.top

ssh user@host 'uptime'
来源：http://vaa.yangfankeji.com

[R58] 下载文件
来源：http://jtt.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kjt.yj20258.top

[R59] 发 POST JSON
来源：http://mig.zhengqikj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qvu.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://jnx.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://akw.cucudq.cn

[R61] 磁盘占用
来源：http://tyi.hongshengwenyu.top

df -h;  du -sh *
来源：http://qmn.wangdashe.top

[R62] 找最占空间的文件
来源：http://vfy.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://nxk.zhongyouzk.top

[R63] 内存与进程
来源：http://nsk.yonumen.top

free -h;  ps aux | grep nginx
来源：http://btu.xuetiantiany.cn

[R64] 结束进程
来源：http://wfc.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://qsi.birdmap.top

[R65] 查看端口占用
来源：http://rfy.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qdr.zhongyouzk.top

[R66] 定时任务
来源：http://szj.yongpay.top

crontab -e;  crontab -l
来源：http://uvf.cashguo.top

[R67] 生成随机十六进制串
来源：http://qgq.yueranfly.top

openssl rand -hex 16
来源：http://nxq.sjlbkw.cn

[R68] 计算文件校验值
来源：http://ggn.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://krv.xylfe.cn

[R69] 生成随机密码
来源：http://wbb.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://kzm.sweek.top

[R70] 时间戳与互转
来源：http://khk.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://qlm.tanke756.top

[R71] 日期格式化
来源：http://jhc.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mui.316326.xyz

[R72] 等待端口就绪
来源：http://nig.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qqw.hfpthk.cn

[R73] 分割大日志
来源：http://nnx.dashuyun.cn

split -l 1000 big.log part_
来源：http://ptv.jyoumei.cn

[R74] 批量重命名
来源：http://mgy.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bam.zhiwuduotai.top

[R75] 导出环境变量
来源：http://lto.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://grl.uphjek.com

[R76] 使用临时文件
来源：http://myu.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eue.jinqigfzy.top

[R77] 读取用户输入
来源：http://qcq.jianghu66.top

read -rp "请输入: " ans
来源：http://feh.daxiang520.top

[R78] 交互式菜单
来源：http://nns.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xar.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://lew.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://klw.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://azq.jinqigufen.top

time ./run.sh
来源：http://kom.zhaomingkeji.xyz

================================================================================
来源：http://hyv.aizwys.cn

S. C / C++ 专题
来源：http://gbi.xziqi.cn

================================================================================
来源：http://oew.xuetiantiany.cn

[S01] C：Hello World
来源：http://frz.yueranfly.top

#include <stdio.h>
来源：http://bxo.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gys.daria6918.cn

[S02] C：变量与格式化输出
来源：http://plu.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://zmu.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://ghd.ehwqpu.com

int x; scanf("%d", &x);
来源：http://unn.yangfankeji.com

[S04] C：字符串复制
来源：http://oww.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://hbz.bbcook.cn

[S05] C：字符串长度
来源：http://ppn.wangdashe.top

strlen(s)
来源：http://odn.svipenyu.cn

[S06] C：字符串比较
来源：http://khb.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://kcg.yangfankeji.com

[S07] C：数组遍历求和
来源：http://gxn.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gsf.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://vuc.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jdn.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://vut.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://miv.sjlbkw.cn

[S10] C：指针与解引用
来源：http://qzx.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://vir.ppjwa.cn

[S11] C：逐行读文件
来源：http://cwv.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://pqe.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://otl.zdqjudy.top

fclose(f);
来源：http://ano.gaohongyu789.top

[S12] C：写文件
来源：http://gju.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://akm.jinqigufen.top

[S13] C：宏定义
来源：http://upz.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yay.havefunace.top

[S14] C：枚举
来源：http://fqf.jinghuilouyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://zlt.52xcode.cn

[S15] C：类型转换
来源：http://csc.daxiang520.top

(double) a / b
来源：http://lba.yj20258.top

[S16] C：位操作置位
来源：http://apx.feifeiyinyue.top

x |= (1 << 3);
来源：http://pbm.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://imr.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bmd.shzxlz.cn

[S18] C：命令行参数
来源：http://ajl.zhengqikj.top

int main(int argc, char **argv)
来源：http://lcp.jinghuilouyu.cn

[S19] C：快速排序
来源：http://sjb.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://xfz.hysaishi.cn

[S20] C：二分查找
来源：http://hia.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vsg.sjlbkw.cn

[S21] C：字符类别判断
来源：http://ils.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tuk.birdmap.top

[S22] C：字符串转数字
来源：http://fvy.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rca.jinghuilouyu.cn

[S23] C：随机数
来源：http://orf.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://srd.redwolf501.top

[S24] C：获取本地时间
来源：http://kxd.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mbn.iojbl.cn

[S25] C：内存拷贝
来源：http://rox.bjfxy.top

memcpy(dst, src, n);
来源：http://emt.xinyue.icu

[S26] C：内存清零
来源：http://enz.yueranfly.top

memset(a, 0, sizeof a);
来源：http://tnv.ppjwa.cn

[S27] C：定义常量
来源：http://kid.hesvh.cn

const double PI = 3.14159;
来源：http://sfl.yfazqb.com

[S28] C：静态变量
来源：http://srt.andypj.xyz


<!-- 参考信息 -->