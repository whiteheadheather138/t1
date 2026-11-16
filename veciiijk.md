代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mpw.yvedp.cn

[Q52] 删除指定行
来源：http://pws.gaohongyu789.top

DELETE FROM users WHERE id = 10;
来源：http://vuo.cheryme.top

[Q53] 按条件删除
来源：http://ylb.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://esg.sxryk.cn

[Q54] 清空表
来源：http://kdc.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://glq.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://hyk.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uul.hesvh.cn

[Q56] 密集排名（并列不占位）
来源：http://rrp.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://avi.jinyuanbaomall.cn

[Q57] 行号
来源：http://fja.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://saq.hesvh.cn

[Q58] 累计求和
来源：http://abp.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wnw.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://yap.dashuyun.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kdw.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://tjw.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sff.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xbr.tarul.cn

[Q61] 移动平均
来源：http://gml.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nnm.pycfn.com

[Q62] 分组占比
来源：http://hra.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mtv.52xcode.cn

[Q63] 开启事务
来源：http://ykd.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gdc.tian-w.cn

[Q64] 提交事务
来源：http://hkn.fehbvm.com

COMMIT;
来源：http://hmf.zycfv.cn

[Q65] 回滚事务
来源：http://ayo.ywan-chungtsiang.top

ROLLBACK;
来源：http://yoh.ydzc1.top

[Q66] 行锁查询
来源：http://ozf.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gff.yj20258.top

[Q67] 设置隔离级别
来源：http://cvq.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://onw.smart0.xyz

[Q68] 保存点
来源：http://yyt.shuidangran.top

SAVEPOINT sp1;
来源：http://hbz.epnwcf.com

ROLLBACK TO sp1;
来源：http://msm.fktsv.cn

[Q69] 查看执行计划
来源：http://zsy.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fdc.iojbl.cn

[Q70] 更新统计信息
来源：http://ffv.yuanzhike.top

ANALYZE TABLE users;
来源：http://jxm.pycfn.com

[Q71] 查看建表语句
来源：http://jul.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://plr.aibaodan.cn

[Q72] 查看索引
来源：http://fdt.redwolf501.top

SHOW INDEX FROM users;
来源：http://jox.meibo888.top

[Q73] 查看表状态
来源：http://mhp.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://uzl.zhoulong.xyz

[Q74] 强制使用索引
来源：http://iqb.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xib.dianchejie.cn

[Q75] 日期格式化
来源：http://pbd.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dzf.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rga.tanke756.top

[Q76] 按天统计
来源：http://qvh.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qzw.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://vkv.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://whn.fengsongda.top

[Q78] 当前时间
来源：http://ufh.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yse.ydzc1.top

[Q79] 字符串拼接
来源：http://qmh.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lrr.9152youxi.cn

[Q80] 字符串截取
来源：http://soq.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://imo.sysykeji.top

[Q81] 字符串替换
来源：http://tuf.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qxx.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://oyd.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://swn.ctjpmb.com

[Q83] 大小写转换
来源：http://wxl.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mpt.hammf.cn

[Q84] 去除首尾空格
来源：http://zxd.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://seg.aizwys.cn

[Q85] 数值取整
来源：http://zoa.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bwz.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://eng.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ele.cucudq.cn

[Q87] JSON 字段做条件
来源：http://gly.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hfs.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://kig.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wuu.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://krd.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://qla.epnwcf.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zdg.hcnkem.com

[Q90] 生成序号列
来源：http://uhn.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cpe.zhaomingkeji.xyz

================================================================================
来源：http://jtl.pycfn.com

R. Bash 专题
来源：http://cch.hnxiangtu.top

================================================================================
来源：http://god.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://vdj.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://zbb.hnxiangtu.top

set -euo pipefail
来源：http://ezh.ppjwa.cn

[R02] 变量赋值与使用
来源：http://ojx.shuidangran.top

name="Tom"; echo "$name"
来源：http://cnu.jyoumei.cn

[R03] 只读变量
来源：http://frd.gaohongyu789.top

readonly PI=3.14
来源：http://jgy.xuanzx.com

[R04] 位置参数
来源：http://aad.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qfb.chenjidiqi.icu

[R05] 参数默认值
来源：http://kra.zhaomingkeji.xyz

name="${1:-default}"
来源：http://hvm.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://xhw.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ioj.hfpthk.cn

[R07] if 判断文件
来源：http://otf.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baq.gotoacloud.top

[R08] 数值比较
来源：http://cok.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mpn.zdbjq.cn

[R09] 字符串比较
来源：http://dhy.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rhx.sxryk.cn

[R10] 正则匹配
来源：http://izj.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://heq.zhijiandao.cn

[R11] case 多分支
来源：http://zax.yanxiufei.cn

case "$1" in
来源：http://swj.feifeiyinyue.top

start) echo "启动" ;;
来源：http://kia.pycfn.com

stop)  echo "停止" ;;
来源：http://nwo.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://jta.chenlongwang.top

esac
来源：http://tdm.316326.xyz

[R12] for 遍历文件
来源：http://fwn.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://fav.hfpthk.cn

[R13] for 计数循环
来源：http://vwl.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://wva.hfpthk.cn

[R14] C 风格 for
来源：http://jxl.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gsc.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://hpi.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gwe.cashguo.top

[R16] until 等待条件
来源：http://gxg.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vxp.pengpengdd.cyou

[R17] 数组定义与取值
来源：http://pbl.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aae.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://cit.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cbg.gaohongyu789.top

[R19] 数组长度
来源：http://iox.hysaishi.cn

echo "${#arr[@]}"
来源：http://rni.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://fli.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jsv.yj202588.top

[R21] 字符串长度
来源：http://dcs.yueranfly.top

echo "${#s}"
来源：http://rsm.hcnkem.com

[R22] 截取子串
来源：http://xsq.chenjidiqi.icu

echo "${s:0:5}"
来源：http://jtd.ppjwa.cn

[R23] 字符串替换
来源：http://pay.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bcz.shuidangran.top

[R24] 大小写转换
来源：http://cer.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://laz.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://hcn.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://snu.yongpay.top

[R26] 命令替换
来源：http://lrd.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://hox.sjlbkw.cn

[R27] 算术展开
来源：http://slj.uphjek.com

echo $((1 + 2 * 3))
来源：http://rkq.hammf.cn

[R28] 浮点运算
来源：http://pjs.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://nbi.hcnkem.com

[R29] 定义函数
来源：http://zmo.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mdv.xinyue.icu

[R30] 函数返回状态码
来源：http://sqt.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://qyq.yangfankeji.com

[R31] 局部变量
来源：http://inx.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://ldy.cdnleiting.top

[R32] 参数个数校验
来源：http://phy.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oad.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://gfg.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yul.yuanzhike.top

[R34] 退出时清理
来源：http://yrl.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cpv.yanxiufei.cn

[R35] 后台执行并等待
来源：http://yjd.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wcz.andypj.xyz

[R36] 并发执行多个任务
来源：http://qre.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wnr.svipenyu.cn

[R37] 把输出赋给变量
来源：http://frc.ctjpmb.com

files=$(ls -1)
来源：http://lqe.jqgufenzy.top

[R38] 管道串联
来源：http://xly.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://sky.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://ttg.andypj.xyz

cmd > out.log 2>&1
来源：http://ujq.uphjek.com

[R40] 追加写日志
来源：http://uhj.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://tqa.chenjidiqi.icu

[R41] 丢弃输出
来源：http://tbv.yongpay.top

cmd >/dev/null 2>&1
来源：http://vzh.jinghuilouyu.cn

[R42] 输入重定向
来源：http://els.tianlin.xyz

wc -l < a.txt
来源：http://qxy.zhoulong.xyz

[R43] 按名字查找文件
来源：http://ggr.yanxiufei.cn

find . -name "*.log" -type f
来源：http://zdk.guannengcc.top

[R44] 按修改时间查找
来源：http://tsv.bjfxy.top

find . -mtime -7 -type f
来源：http://biq.zdbjq.cn

[R45] 批量删除
来源：http://gni.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://wlk.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://yvw.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tar.shuidangran.top

[R47] sed 单行替换
来源：http://gnu.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://jka.nwbrower.top

[R48] awk 取指定列
来源：http://nuo.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://rqn.ctjpmb.com

[R49] awk 带条件
来源：http://ite.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ryi.iojbl.cn

[R50] awk 求和
来源：http://xnf.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://ibq.vehdjk.com

[R51] 排序去重取前几
来源：http://evn.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tju.jinqigufen.top

[R52] 统计行数
来源：http://tcg.dashuyun.cn

wc -l a.txt
来源：http://qmg.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://amh.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://scf.zdbjq.cn

[R54] 比较两个文件
来源：http://mey.andypj.xyz

diff a.txt b.txt
来源：http://vsx.gzhubu.top

[R55] 压缩与解压
来源：http://bdp.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fnq.sysykeji.top

[R56] 远程拷贝
来源：http://sez.jqgfzy.top

scp file user@host:/path/
来源：http://lzf.tian-w.cn

[R57] 远程执行命令
来源：http://knp.havefunace.top

ssh user@host 'uptime'
来源：http://slh.daria6918.cn

[R58] 下载文件
来源：http://jdi.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qer.nanxinkj.top

[R59] 发 POST JSON
来源：http://iet.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rgc.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://hwh.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ldv.jiagoushi.top

[R61] 磁盘占用
来源：http://bzu.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://wpv.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://ekp.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://lws.feifeiyinyue.top

[R63] 内存与进程
来源：http://oik.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://kxn.mhx1999.top

[R64] 结束进程
来源：http://zkb.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://rjk.ivvv.top

[R65] 查看端口占用
来源：http://qki.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gze.aizwys.cn

[R66] 定时任务
来源：http://svb.aibaodan.cn

crontab -e;  crontab -l
来源：http://zjg.ivvv.top

[R67] 生成随机十六进制串
来源：http://omy.yfazqb.com

openssl rand -hex 16
来源：http://qle.daxiang520.top

[R68] 计算文件校验值
来源：http://ecs.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://yvw.bjfxy.top

[R69] 生成随机密码
来源：http://hir.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://uuw.zycfv.cn

[R70] 时间戳与互转
来源：http://gah.xylfe.cn

date +%s;  date -d @1700000000
来源：http://kmf.fzhhl.top

[R71] 日期格式化
来源：http://llx.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mbb.0kj1m.cn

[R72] 等待端口就绪
来源：http://xks.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://imo.sweek.top

[R73] 分割大日志
来源：http://bih.guannengcc.top

split -l 1000 big.log part_
来源：http://edb.iojbl.cn

[R74] 批量重命名
来源：http://jpz.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xdl.zhijiandao.cn

[R75] 导出环境变量
来源：http://udu.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://opo.zhengqikj.top

[R76] 使用临时文件
来源：http://esb.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ckk.fengsongda.top

[R77] 读取用户输入
来源：http://hgn.hnqzz.top

read -rp "请输入: " ans
来源：http://ykr.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://adw.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vmi.birdmap.top

[R79] 解析命令行选项
来源：http://fzd.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://geq.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://lgh.vqdsnc.cn

time ./run.sh
来源：http://odm.sysykeji.top

================================================================================
来源：http://bbv.gogol.net.cn

S. C / C++ 专题
来源：http://fje.hongshengwenyu.top

================================================================================
来源：http://jwq.bjfxy.top

[S01] C：Hello World
来源：http://jvi.ybcxt.top

#include <stdio.h>
来源：http://mvn.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nft.yvedp.cn

[S02] C：变量与格式化输出
来源：http://gmv.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://nei.sweek.top

[S03] C：读入整数
来源：http://tph.hammf.cn

int x; scanf("%d", &x);
来源：http://hfe.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://qlz.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://egd.9152youxi.cn

[S05] C：字符串长度
来源：http://mhw.cashguo.top

strlen(s)
来源：http://pvj.dianchejie.cn

[S06] C：字符串比较
来源：http://iop.52xcode.cn

strcmp(a, b) == 0
来源：http://nfy.316326.xyz

[S07] C：数组遍历求和
来源：http://tjq.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tao.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://pdr.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sno.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://ixf.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zuk.ybcxt.top

[S10] C：指针与解引用
来源：http://xnp.fktsv.cn

int *p = &a;  *p = 5;
来源：http://zqo.jqgufenzy.top

[S11] C：逐行读文件
来源：http://fbl.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://wfn.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://jtv.xziqi.cn

fclose(f);
来源：http://aat.sjlbkw.cn

[S12] C：写文件
来源：http://cwf.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ppn.316326.xyz

[S13] C：宏定义
来源：http://jix.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vmv.feifeiyinyue.top

[S14] C：枚举
来源：http://jyl.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://iay.hnxiangtu.top

[S15] C：类型转换
来源：http://plj.nwbrower.top

(double) a / b
来源：http://yyb.ivvv.top

[S16] C：位操作置位
来源：http://vry.ivvv.top

x |= (1 << 3);
来源：http://qiv.yuxming.cn

[S17] C：安全拼接字符串
来源：http://nxa.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ayq.yfazqb.com

[S18] C：命令行参数
来源：http://hyu.fengsongda.top

int main(int argc, char **argv)
来源：http://kcp.aizwys.cn

[S19] C：快速排序
来源：http://dii.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://crb.bjfxy.top

[S20] C：二分查找
来源：http://rof.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://smg.zhoulong.xyz

[S21] C：字符类别判断
来源：http://jke.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://alx.smart0.xyz

[S22] C：字符串转数字
来源：http://xrh.wangdashe.top


<!-- 参考信息 -->